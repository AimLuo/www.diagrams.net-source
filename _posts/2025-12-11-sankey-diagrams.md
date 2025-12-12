---
layout: post
author: draw.io
slug: sankey-diagrams
date: 2025-12-11 09:43:00
title: Four ways to draw Sankey diagrams in draw.io
tags: [shape libraries]
categories: [use-cases]
---

Sankey diagrams were originally designed to visualise loss in a steam engine system. These days, they are also used to illustrate data distributions and flows between states in many types of systems. 
<br /><img src="/assets/img/blog/sankey-boiler-shapes.png" style="width=100%;max-width:500px;height:auto;" alt="A Sankey diagram of a steam engine drawn in draw.io using shapes for the links">
<br />[_Open this example_](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&page=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fsankey-diagrams.drawio)

[Sankey diagrams](https://en.wikipedia.org/wiki/Sankey_diagram) and their related [alluvial diagrams](https://en.wikipedia.org/wiki/Alluvial_diagram) and [flow maps](https://en.wikipedia.org/wiki/Flow_map) can visualise:
* Movement of energy, resources, or materials through a system
* Migration flows between different locations
* Budgets and financial modelling
* User journeys through multiple platforms or system states
* Waste visualisations in manufacturing
* Traffic (both physical and digital) over time
* Decisions leading to and from certain states (such as for medical diagnoses)

The different stages or states in a Sankey diagram are called _nodes_, and are often drawn as vertical lines into and out of which the _links_ (connections) flow and split to the next stage.
<br />[<img src="/assets/img/blog/sankey-budget.png" style="width=100%;max-width:400px;height:auto;" alt="A Sankey diagram for a simple budget">](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&page=3&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fsankey-diagrams.drawio)
<br />[_Open this example_](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&page=3&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fsankey-diagrams.drawio)

The first Sankey diagram, named after its creator who drew it in 1898, shows the energy flow through an ideal and actual steam engine. He used regions (square boxes) rather than vertical lines to represent each stage. 
<br />[<img src="/assets/img/blog/sankey-boiler-connectors.png" style="width=100%;max-width:400px;height:auto;" alt="A Sankey diagram of an ideal steam engine drawn in draw.io using connectors for the links">](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&page=0&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fsankey-diagrams.drawio)
<br />[_Open this example_](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&page=0&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fsankey-diagrams.drawio)

If you don't need a value-accurate representation of your system, there are a few ways to draw Sankey diagrams in draw.io. For a Sankey diagram directly from your data, use Mermaid code and insert that into draw.io for an accurate visualisation.

## Method 1: Use connectors for curves

The fastest and perhaps easiest way is to use the _partial rectangle_ shape in the _Misc_ shape library for the horizontal and vertical links.
 <br /><img src="/assets/img/blog/sankey-partial-rectangle.png" style="width=100%;max-width:400px;height:auto;" alt="Use partial rectangle shapes in your Sankey diagram and attach curved connectors to their corners">

Use curved connectors and attach them to the corners of the partial rectangles.
 <br /><img src="/assets/img/blog/sankey-curved-connectors.png" style="width=100%;max-width:400px;height:auto;" alt="Use partial rectangle shapes in your Sankey diagram and attach curved connectors to their corners">

The corners of the partial rectangles perfectly align with the curved connectors, giving your diagram a neat finish. 

**Use layers for better diagram management**

Add directional flow arrows on a separate layer. It makes it much easier to edit and label your diagram when you can lock the layers you aren't working with to prevent any miss-editing. 

Place regions on a separate layer on top and use the hatch fill style so you can see the underlying flows of your system clearly.
<br /><img src="/assets/img/blog/sankey-regions.png" style="width=100%;max-width:400px;height:auto;" alt="Use the hatch fill style on regions so the flows below can still be seen">

[_See how to use layers in diagrams_](/doc/layers.html)

**Join connectors with waypoint shapes** 

Where two curves join, use a [waypoint shape](/blog/waypoint-shape.html) to keep them attached. Disable the waypoint shape's _Line_ to turn the shape invisible.
 <br /><img src="/assets/img/blog/sankey-waypoint-shape.png" style="width=100%;max-width:400px;height:auto;" alt="Disable the Line checkbox in the Style tab to make a waypoint shape invisible">

## Method 2: Use filled edges for coloured connectors

By using individual connectors to attach the curves to the corners of the partial rectangles, you _can't add a fill colour_ to the entire system - the space between the two connectors on the curves is not a shape and therefore can't be filled. 

The _filled edge_ shape from the _Misc_ shape library is routed and attached to shapes as a connector and filled with colour like a shape. 
<br /><img src="/assets/img/blog/sankey-filled-edge.png" style="width=100%;max-width:500px;height:auto;" alt="A Sankey diagram of a budget using the filled edge shape">

This is an ideal way to create budget flows or similar data-based distribution diagrams.
1. Add a _fork/join_ shape to the canvas and make it 100 points tall in the _Arrange_ tab of the format panel - enter ``Fork`` in the [shape search](/doc/faq/shape-search.html) to find the fork shape. 
<br /><img src="/assets/img/blog/sankey-fork-shape.png" style="width=100%;max-width:500px;height:auto;" alt="Add a fork shape from the shape search to represent a stage in a Sankey diagram in draw.io">
2. Change the width of each filled edge to be the percentage for each particular category.
 <br /><img src="/assets/img/blog/sankey-budget-distribution.png" style="width=100%;max-width:350px;height:auto;" alt="A Sankey diagram where each flow is a percentage - represented by the connector width value">
1. Attach the connectors to the line or fork shape - they should stack up perfectly to cover the entire length of the 100pt high fork shape. 
2. Use the _Entity Relation_ connector shape to fan out the flows neatly.

As this is a connector and not a shape, the right/left labels settings do not move the text far from the centre of the connector. Drag the orange diamonds to line each label of the filled edge shapes so they are lined up and easily readable. 
<br /><img src="/assets/img/blog/sankey-filled-edge-labels.png" style="width=100%;max-width:300px;height:auto;" alt="Drag the labels of the filled edge in a Sankey diagram using the orange diamond grab handle">

**Note:** It can be difficult to get the filled edge shapes to line up with the outlines of partial rectangle shapes. If you want to fill your entire system with colours, and filled edges are proving too difficult to use, use _partial concentric ellipse_ or _arrow_ shapes for the curves.

## Method 3: Use shapes for curves

In this method, there are no attached connectors - your Sankey diagram will be a collection of shapes drawn right next to each other and positioned just right so it appears to be one flowing system of pipes.

**Using arrow shapes**

The _U-turn arrow_ and _bend arrow_ shapes from the _Arrows_ shape library are useful for curves. Drag the orange diamonds to remove the arrow heads and turn them into a pipe shape, then use fill colours as you would in any normal shape. 
<br /><img src="/assets/img/blog/arrow-shape-remove-head.gif" style="width=100%;max-width:400px;height:auto;" alt="Remove the arrow heads with the orange diamond grab handles to create a bent pipe shape from an arrow shape">

They do have a minimum width, however, and may not be suitable for small or fine flows.


**Using a partial concentric ellipse or arc shape**

The _partial concentric ellipse_ shape_ from the _Basic_ shape library is more flexible - drag the orange diamonds to change thickness and arc segment. Rotate to line up with the partial rectangle shapes. 

Make sure you enable the _Constrain Proportions_ checkbox in the _Arrange_ tab of the format panel to resize without distorting the arc width. 
<br /><img src="/assets/img/blog/partial-concentric-ellipse.gif" style="width=100%;max-width:500px;height:auto;" alt="Drag the orange diamond grab handles to change the thickness and arc segment of the partial concentric ellipse shape and enable the Constrain Proportions checkbox in the Arrange tab to resize it neatly">

Rotate the shapes so they butt up against or slightly overlap the partial rectangles and bring the partial rectangles to the front via the _Arrange_ tab or right-click context menu to cover the outline and 'connect' the pipes.
 <br /><img src="/assets/img/blog/sankey-to-front.png" style="width=100%;max-width:300px;height:auto;" alt="Slightly overlap the curved shapes with the partial rectangles and bring the rectangles to the front via the Arrange tab in the format panel to hide the outline and join the 'pipes'">

With this method, you can add fill colours to enhance your diagram.
* use gradient colours in curves and links to indicate state changes between nodes
* use different colours for different paths

[<img src="/assets/img/blog/sankey-boiler-shapes.png" style="width=100%;max-width:500px;height:auto;" alt="A Sankey diagram of a steam engine drawn in draw.io using shapes for the links">](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&page=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fsankey-diagrams.drawio)
<br />[_Open this example_](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&page=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fsankey-diagrams.drawio)


## Method 4: Draw Mermaid Sankey diagrams

draw.io is not a data visualisation platform, but it can take the experimental Mermaid descriptions of Sankey diagrams with specific values for each link and convert that code to an SVG diagram. 

The example below has been inserted into draw.io from the [Mermaid documentation](https://mermaid.js.org/syntax/sankey.html). 
* Click _Arrange > Insert > Mermaid_ and add the Mermaid code to the text box. 
* Click _Insert_ to add the diagram to the drawing canvas as a SVG shape.
<br />[<img src="/assets/img/blog/sankey-mermaid.png" style="width=100%;max-width:500px;height:auto;" alt="A Sankey diagram of electricity generation and usage from and to different categories">](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&page=2&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fsankey-diagrams.drawio)
<br />[_Open this example_](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&page=2&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fsankey-diagrams.drawio)

draw.io does not convert Mermaid Sankey diagrams to native draw.io shapes. Hover over the diagram to see the Mermaid code and double click on it to edit the code and regenerate the diagram. 

## Related

**Flow maps** are similar to Sankey diagrams in that they show the distribution of traffic, such as [this old map of Irish railroad traffic](https://en.wikipedia.org/wiki/File:Harness_Ireland_Railroad_Map_1838.png), drawn by Henry Harness in 1838. 

To create a similar diagram in draw.io: 
1. Drag and drop an image of the map in a background layer on the drawing canvas and resize it appropriately. 
2. Lock that layer and create a new one. 
3. On the new layer, add [waypoint shapes](/blog/waypoint-shape.html) at key locations to join or split connectors. 
4. Then draw the flows with connectors of varying widths.

