---
title: Week 1
published: 2024-06-03
tags: [GSOC]
category: GSOC
draft: false
---

# Week 1 at GSOC: Exploring 3D Visualization for LabPlot

As I wrap up my first week of the Google Summer of Code (GSOC) project with LabPlot, I'm excited to share my progress and insights. My project aims to extend LabPlot's visualization capabilities from 2D to 3D plotting, a crucial step in meeting the evolving needs of scientific research.

## The Project Goal

LabPlot is already well-known for its powerful 2D visualization features, including various plot types like line, scatter, and their variations. However, the scientific community increasingly requires 3D visualization tools. My GSOC project focuses on bridging this gap by introducing 3D plotting capabilities to LabPlot.

## Week 1: Exploring Options

This week, I dove deep into researching and evaluating different libraries and tools that could potentially power LabPlot's 3D plotting feature. The main contenders were:

| Library/Tool   | Advantages                                                                                          | Disadvantages                                                                                   |
|----------------|-----------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|
| VTK/ParaView   | Powerful 3D visualization capabilities, widely used                                                    | Heavy dependency, limited interactivity compared to LabPlot's current interface                |
| Mayavi         | Powerful visualization, Python-based                                                                 | Similar drawbacks as VTK in terms of integration complexity and interactivity limitations     |
| QtGraphs       | Seamless Qt integration, maintains consistency with LabPlot's codebase, high interactivity           | Lightweight compared to VTK, minimal , lack certain 3D Plots ex:- line plot                                            |

### The Decision

Based on this week's exploration and analysis, we've decided to move forward with **QtGraphs** for implementing 3D plotting in LabPlot. This choice allows us to maintain LabPlot's highly interactive nature while expanding its capabilities into the 3D ploting.

## Next Steps

In the coming weeks, I'll be diving deeper into QtGraphs, learning its API, and starting to design how we'll integrate 3D plotting into LabPlot's existing interface. I'm excited about the challenges ahead and the potential impact this project will have on LabPlot's users in the scientific community.

Stay tuned for more updates as we progress through this exciting journey of bringing 3D visualization to LabPlot!
---
