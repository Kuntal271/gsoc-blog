---
title: Week 2
published: 2024-06-12
description: Implementing a Basic 3D Scene in LabPlot.
tags: [GSOC]
category: GSOC
draft: false
---

# Week 2 at GSOC: Implementing a Basic 3D Scene in LabPlot

As I conclude my second week of the Google Summer of Code (GSOC) project with LabPlot, I'm excited to share the progress we've made in implementing 3D visualization capabilities. This week has been filled with exploration, decision-making, and tackling some interesting challenges.

## Exploring QtGraphs APIs

After deciding to use QtGraphs for our 3D plotting implementation, I spent a significant portion of this week diving deep into its APIs. This exploration was crucial for understanding how we can best integrate 3D plotting into LabPlot's existing structure.

## Implementing a Basic 3D Scene

Our main goal for this week was to implement a basic 3D scene on a worksheet. This milestone represents the first concrete step towards bringing 3D visualization to LabPlot.

## Switching to QtGraphs 6.7.1

During our implementation process, we made an important discovery. The recently released QtGraphs 6.7.1 has introduced some significant changes in the implementation of basic 3D plots. One of the most notable changes is that QAbstract3DGraph now inherits from QWidget instead of QWindow as in earlier versions.

This change turned out to be advantageous for our project. In previous versions, adding a QWindow to a QGraphicsScene was a cumbersome process. The shift to QWidget in the new version aligns better with LabPlot's existing architecture, making the integration process smoother.

## Challenges Faced

While the new version of QtGraphs solved some problems, it also presented new challenges:

- **Adding QWidgetProxy to QGraphicsScene:** Integrating the 3D scene into LabPlot's existing QGraphicsScene required careful implementation of QWidgetProxy.
- **Handling Scene Events:** A significant challenge was making the QProxyWidget accept scene events like rotation, scaling, and translation of the 3D scene using mouse inputs.

These challenges required a deep dive into Qt's event handling mechanisms and how they interact with QtGraphs' 3D scene implementation.

## Solutions and Progress

Despite these challenges, we made significant progress:

- We successfully implemented a basic 3D scene within a LabPlot worksheet.
- We developed a solution for adding the 3D scene to the QGraphicsScene using QWidgetProxy.
- We're in the process of fine-tuning the event handling to ensure smooth interaction with the 3D scene using mouse inputs.

## Next Steps

As we move into the third week, our focus will be on:

- Refining the event handling for the 3D scene to ensure smooth user interaction.
- Expanding the types of 3D plots available, starting with basic scatter and surface plots.
- Integrating the 3D plotting capabilities with LabPlot's data handling mechanisms.

The progress we've made this week is exciting, and I'm looking forward to overcoming the remaining challenges. Stay tuned for more updates as we continue to enhance LabPlot's visualization capabilities!

