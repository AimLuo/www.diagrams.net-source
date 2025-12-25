---
title: Work with connectors
layout: page
faq: true
categories: [Connectors]
---

连接线是连接形状的线条。它们也可以在一端或两端有箭头或其他符号。

draw.io 中有两种类型的连接线。

## 浮动和固定连接线

draw.io 中有两种主要类型的连接线。

* **浮动连接线**围绕形状的周边移动。
* **固定连接线**保持连接到形状上的固定点。 
<br /><img src="/assets/img/blog/connector-floating-vs-fixed.gif" style="width=100%;max-width:400px;height:auto;" alt="Floating connectors move intelligently around the shape when you move it. Fixed connectors stay attached to that fixed point on the shape.">

连接线可以一端固定，另一端浮动，或者两端使用相同类型的连接。 

### Add a floating connector

1. Hover over an existing shape, then click and drag a connector from one of the four directional arrows.
2. Hover over the target shape, then drop the connector end when the shape outline is blue. 
<br /><img src="/assets/img/blog/connector-floating.png" style="width=100%;max-width:300px;height:auto;" alt="Floating connector - Drop the connector on the target shape when the outline is blue">

Floating connectors will take the shortest route between the two shapes, unless you manually change the path they take by adding waypoints (learn more about waypoints below).

### Add a fixed connector 
1. Hover over a shape to see the fixed connection points - they look like small crosses.
2. Hover over one of these points, then click and drag a connector from it.
3. Hover over a connection point on the target shape, then drop the connector when it is highlighted in green to make it into a fixed connection.
<br /><img src="/assets/img/blog/connector-fixed.png" style="width=100%;max-width:300px;height:auto;" alt="Fixed connector - Drop the connector on a connection point - a small x - when it is highlighted with a green circle">

You can [fix the end of a connection to any location within a shape](/doc/faq/connect-to-shapes-anywhere.html).

Fixed connectors will remain attached to that particular location on a shape, even when you rotate the shape, or move it (or the connector) around the drawing canvas.

**Tip:** Click on the direction arrow pointing towards a nearby shape to quickly connect the two.
<br /><img src="/assets/img/blog/connector-direction-arrow.png" style="width=100%;max-width:250px;height:auto;" alt="Click on a direction arrow near a neighbouring shape to connect it">

* [Edit the fixed connection points on a shape](/blog/edit-connection-points.html)
* [Make floating connectors snap to the nearest fixed connection point](/blog/snap-to-point.html). 
* [Customise a shape to have different connection points](/doc/faq/shape-connection-points-customise.html)
* [Learn how to use waypoints to change the connector's path](/blog/waypoints-connectors.html)

## 自动连接形状

draw.io 编辑器可以在您向绘图画布添加新形状时以多种方式自动添加连接线。

**克隆并连接形状：** 单击指向绘图画布上空白区域的方向箭头，然后选择一个形状以在该方向上添加并连接它。

**拖放形状：** 从形状库或绘图画布拖动形状，并将其放在方向箭头或现有的未连接连接线上。

<img src="/assets/img/blog/shapes-clone-add-connect.gif" style="width=100%;max-width:300px;height:auto;" alt="Drag and drop shapes onto the blue directional arrows or connector ends">

[Use shortcuts to add, clone and automatically connect shapes](/blog/connect-shapes.html)

## 向连接线添加标签

连接线可以有三个标签 - 一个在中间，一个在两端。

在要添加标签的位置双击连接线。

当您在绘图画布上移动形状时，这些标签会随连接线移动，但您也可以将它们拖动到另一个位置。
* 要手动更改标签的位置，请通过单击选择标签，然后将菱形抓取手柄拖动到新位置。
<br /><img src="/assets/img/blog/connector-label.png" style="width=100%;max-width:400px;height:auto;" alt="Connectors can have three labels - double click to add a label to a connector, and drag the labels to a new position using the diamond grab handle.">

## Use waypoints on connectors

Connectors use waypoints as anchors for their route between two shapes. These are displayed as round blue grab handles. 

<img src="/assets/img/blog/connector-waypoints.png" style="width=100%;max-width:300px;height:auto;" alt="Use waypoints to change the path of your connector across the drawing canvas">

Waypoints are useful when you want to ensure a connector takes a certain path, especially when it is a floating connector which will default to the shortest, direct route.

To add or remove waypoints and change the path of a connector, drag a section of the connector into a new position to make it take a different route. Waypoints are added and removed automatically as you drag them into new positions. 

<img src="/assets/img/blog/waypoints-add.gif" style="width=100%;max-width:300px;height:auto;" alt="Drag a connector to add waypoints">

**Add extra waypoints manually** - right-click on the connector, then select _Add Waypoint_ from the context menu. 

[See how to remove waypoints](/doc/faq/add-remove-waypoints.html)

**Tip:** You can [reverse the source and target ends of a connector](/doc/faq/connector-reverse.html) (with their labels), and [flip a connector horizontally or vertically](/doc/faq/connector-flip.html) via the _Arrange_ tab in the format panel.

## 将连接线移动到形状的前面或后面

**将连接线直接移动到前面或后面**

1. 选择一个或多个连接线。
2. 单击_置于顶层_或_置于底层_以将它们直接发送到该图层上所有形状和连接线的前面或后面。

**向前或向后移动连接线**

1. 选择一个连接线或一组形状/连接线。
2. 单击_上移一层_或_下移一层_以一次一个形状地向前或向后移动选定的连接线。
<br /><img src="/assets/img/blog/arrange-tab-connector-bring-forward.gif" style="width=100%;max-width:400px;height:auto;" alt="Move connectors in front of or behind other shapes and connectors using the tools on the Arrange tab">

[Learn more about the z-order of shapes and layers](/blog/move-shapes-forwards-backwards.html)

## 连接线样式选项

您可以通过多种不同的方式设置连接线的样式。
* 更改线条颜色、不透明度、宽度和图案。
* 将弯曲设置为锐角、圆角或曲线。
* 使用各种路径点样式更改自动路由行为。
* 添加各种不同的箭头或技术符号。
* 在形状边界外开始或结束连接线，或在形状内偏移它。
* 设置重叠线条使用线跳。
* 以随意的草图样式绘制连接线，带或不带阴影。

要更改连接线的样式，请选择连接线，然后使用格式面板的``样式``选项卡中的选项或工具栏中的工具。

[Learn all about connector styles in draw.io](/doc/faq/connector-styles.html)

<img src="/assets/img/blog/connector-style-tools.png" style="width=100%;max-width:400px;;height:auto;" alt="The Style tab in the format panel and the connector tools in the tool bar let you change the style of a selected connector in draw.io">