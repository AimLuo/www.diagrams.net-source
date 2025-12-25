---
title: Draw a basic flow chart in draw.io
layout: page
categories: [features]
---

您可以使用 draw.io 和[我们的在线图表编辑器](https://app.diagrams.net)创建许多不同类型的图表。要学习如何使用编辑器，让我们从一个基本的[流程图](/example-diagrams.html#flowcharts)开始来记录流程。

流程图让您直观地描述流程或系统。形状和非常简短的标签让读者快速了解他们需要做什么。

[<img src="/assets/img/blog/tutorial-new-diagram-header.png" style="width=100%;max-width:90px;" alt="Create a new diagram in draw.io">](#create-a-new-blank-diagram) [<img src="/assets/img/blog/tutorial-add-shapes-header.png" style="width=100%;max-width:90px;" alt="Add shapes in the draw.io editor">](#add-shapes-to-the-drawing-canvas) [<img src="/assets/img/blog/tutorial-edit-shapes-header.png" style="width=100%;max-width:90px;" alt="Edit shapes on the draw.io drawing canvas">](#move-resize-rotate-and-delete-shapes) [<img src="/assets/img/blog/tutorial-connect-shapes-header.png" style="width=100%;max-width:90px;" alt="Draw connectors between shapes in the draw.io editor">](#connect-shapes) [<img src="/assets/img/blog/tutorial-add-labels-header.png" style="width=100%;max-width:90px;" alt="Add labels to shapes and connectors in draw.io">](#connect-shapes) [<img src="/assets/img/blog/tutorial-style-diagram-header.png" style="width=100%;max-width:90px;" alt="Style shapes, connectors and text in draw.io">](#style-your-flow-chart) [<img src="/assets/img/blog/tutorial-export-header.png" style="width=100%;max-width:90px;" alt="Export and share your diagram created in draw.io">](#connect-shapes)

**教程：** 创建并设置_基本流程图_的样式以学习 draw.io 编辑器。

- [Create a new blank diagram](#create-a-new-blank-diagram)
- [Add shapes to the drawing canvas](#add-shapes-to-the-drawing-canvas)
- [Move, resize, rotate, and delete shapes](#move-resize-rotate-and-delete-shapes)
- [Connect shapes](#connect-shapes)
  - [Draw a floating connector](#draw-a-floating-connector)
  - [Draw a fixed connector](#draw-a-fixed-connector)
  - [Change the path of a connector](#change-the-path-of-a-connector)
- [Add labels](#add-labels)
- [Style your flow chart](#style-your-flow-chart)
- [Export and share your flow chart](#export-and-share-your-flow-chart)

## 创建新的空白图表

1. 转到[在线 draw.io 编辑器](https://app.diagrams.net)。
2. 单击_创建新图表_。
<br /><img src="/assets/img/blog/basic-flow-create-new-diagram.png" style="width=100%;max-width:200px;height:auto;" alt="Click Create New Diagram to start a new diagram">
1. 在模板管理器中，为流程图输入文件名，确保选择了_空白图表_，然后单击_创建_。
<br /><img src="/assets/img/blog/basic-flow-create-blank-diagram.png" style="width=100%;max-width:300px;height:auto;" alt="Enter a filename, select Blank Diagram, and click Create">

**提示：** 如果您想[将图表保存到其他位置](/doc/faq/storage-location-select.html)，请先单击_更改存储位置_。 

<br />
## 向绘图画布添加形状

在 draw.io 中有多种方法可以向绘图画布添加形状。

**添加第一步** - 使用以下方法之一将矩形添加到绘图画布。矩形表示流程中的步骤。

* 单击_常规_形状库中的矩形以将其添加到绘图画布。
* 双击绘图画布上的空白区域并选择矩形形状。
* 从_常规_形状库将矩形拖到绘图画布上的特定位置。

<img src="/assets/img/blog/basic-flow-add-shape.gif" style="max-width:100%;height:auto;" alt="Add a rectangle - click on it in the shape library, double click on a blank area, or drag it from the shape library">

**Add more shapes** - Use one of the following methods to add extra shapes to represent the next steps in your process.
* Hover over the first shape you placed to see the four direction arrows. Click on one of the shapes, then select a shape to add and connect it in that direction.
* Drag a shape from the shape library and hover over an existing shape until you can see the four direction arrows. Move over one of these direction arrows, and drop the shape you have dragged. It will be added to the drawing canvas and connected in that direction.

<img src="/assets/img/blog/basic-flow-add-connect-shape.gif" style="max-width:100%;height:auto;" alt="Add a second shape and connect it from the first - hover and click on the direction arrow, or drag a shape over another and drop it on a direction arrow">

If you added multiple shapes by simply clicking on them in the shape library, you can connect them later. See [how to connect shapes below](#connect-shapes).

**流程图的形状**

流程图中有许多不同的形状用于可视化流程。

* **矩形** - 流程中的基本步骤。
* **菱形** - 决策，通常是是/否问题，将流程分成两个或多个分支。
* **圆形或椭圆形** - 流程中的可选起点和终点。
* **平行四边形** - 输入或输出，流程需要或向外部方或系统提供信息。
* **圆柱体** - 磁盘驱动器，用于指示在该流程步骤中存储数据。
* **底部带波浪线的矩形** - 作为流程步骤的结果生成的文档。

<img src="/assets/img/blog/flow-chart-shapes.png" style="max-width:100%;height:auto;" alt="A selection of shapes available in draw.io commonly used in flow charts">

除了_常规_和_高级_形状库中的形状外，您还可以使用_流程图_形状库中的形状。

1. 单击左侧面板底部的_更多形状_。
2. 单击_流程图_形状库名称旁边的复选框以启用它。
<br /><img src="/assets/img/blog/shape-library-dialog.png" style="width=100%;max-width:300px;height:auto;" alt="Select the shape libraries you want to work with in draw.io">
3. 单击_应用_。_流程图_形状库现在在左侧面板中可用。

<br />
## Move, resize, rotate, and delete shapes

To select a shape, click on it. To [select multiple shapes](/doc/faq/select-multiple-shapes.html), hold down ``Shift`` or ``Cmd`` and click on them.

**Move** - Select and drag a shape that is on the drawing canvas to another position.

**Resize** - Select a shape. Drag any of the round 'grab' handles to make the shape smaller or larger. Hold down ``Control`` when you resize shapes to keep them centred.
<br />[See how to resize groups of shapes](/doc/faq/shape-resize.html)

**Rotate** - Select a shape. Drag the rotate grab handle (the round arrow) at the top right corner of the shape to [rotate the shape](/blog/rotate-shapes.html) around its center point.
<br /><img src="/assets/img/blog/rotate.png" style="width=100%;max-width:300px;height:auto;" alt="Rotate a shape using the rotate grab handle">

**Delete** - Select a shape, then press ``Backspace`` or ``Delete``, or click on the _Delete_ tool in the toolbar.

<img src="/assets/img/blog/basic-flow-move-resize-rotate-delete.gif" style="width=100%;max-width:400px;height:auto;" alt="Move, resize, rotate and delete shapes in draw.io">

If one of the connectors, the arrows between the shapes, is going in the wrong direction, you can select and delete it, just like a shape. Follow the steps below to [draw a new connector](#draw-a-floating-connector) so it goes in the right direction.

**Tip:** Use the _Arrange_ tab to [precisely rotate, reposition and resize shapes](/doc/faq/arrange-tab.html)

<br />
## 连接形状

连接线是[将形状连接在一起](/blog/connect-shapes.html)的线条，可能在一端或两端有箭头，也可能没有箭头。有两种类型的连接线。

**浮动连接线** - 当您在绘图画布上移动形状或更改连接线路径时，这些连接线会围绕形状的周边移动。

**固定连接线** - 这些连接线保持连接到形状上的固定点，即使您在绘图画布上移动形状也是如此。

### Draw a floating connector

1. Hover over the source shape until you see the light direction arrows appear.
2. Move your mouse cursor over the direction arrow you want to draw the connector from, then drag the connector out from the arrow towards the target shape.
3. Hover over the target shape and release when the outline of the shape is blue.

<img src="/assets/img/blog/basic-flow-floating-connector.gif" style="width=100%;max-width:400px;height:auto;" alt="Draw  a floating connectors between shapes in draw.io">

When you move the shape to a new position, the connector ends will automatically move around the shape to ensure the shortest distance.

### Draw a fixed connector

1. Hover over the source shape until you see the little crosses, connection points, around the shape perimeter.
2. Drag a connector from the connection point on the source shape towards the target shape.
3. Hover over the target shape until you see the connection points, then hover over one of the connection points until it is highlighted in green, and release to attach the connector.

<img src="/assets/img/blog/basic-flow-fixed-connector.gif" style="width=100%;max-width:400px;height:auto;" alt="Draw  a fixed connectors between shapes in draw.io">

Now when you drag the shape around on the drawing canvas, the connector will remain attached to exactly those connection points.

### Change the path of a connector

Waypoints are shown as small circles on a selected connector. They are used to define the path that a connector takes across the drawing canvas.

1. Select the connector that you want to change the path of to see its waypoints.
2. Drag one of the waypoints into a new position. New waypoints will be added automatically based on where you grabbed the connector and where you move your mouse too.

If it is a floating connector, the end closest to the waypoints you moved will 'float' around the perimeter of your shape. If it is a fixed connector, the end will remain attached to that specific connection point.

<img src="/assets/img/blog/basic-flow-move-connector.gif" style="width=100%;max-width:400px;height:auto;" alt="Change the path of a connector between shapes in draw.io">

You can [add and remove waypoints](/blog/waypoints-connectors.html) to make connectors follow complex paths.

[Learn more about working with and styling connectors](/doc/faq/connectors.html)

<br />
## Add labels

Short labels on shapes make it easier to understand a diagram quickly.

1. Double click on a shape. Start typing to replace the label with your own text. Alternatively, single click on a shape and start typing to add or edit the label.
2. Press ``Enter`` to save the label text.

**Tip:** Press ``Shift+Enter`` to [add a line break in a label](/doc/faq/line-breaks.html).

<img src="/assets/img/blog/basic-flow-add-labels.gif" style="width=100%;max-width:500px;height:auto;" alt="Add labels to shapes and connectors in draw.io">

**Connector labels**

You can add more than one label to a connector - at the source end, the target end, and in the middle.

* Double click in the position you want to add a text label there.
* To reposition the connector label text, click on the label, then drag the small yellow diamond to a new position.

If you reroute the connector, you may need to update any labels you had manually positioned, but usually the label will move intelligently with the connector.

<br />
## Style your flow chart

Once you have finished adding all the shapes, connectors and labels, you can style your flow chart.

1. Select a shape, or hold ``Shift`` down and click on multiple shapes and connectors to select many.
<br /><img src="/assets/img/blog/basic-flow-style-diagram.gif" style="width=100%;max-width:500px;height:auto;" alt="Add colours, styles and change fonts to make your diagrams more attractive in draw.io">
2. Add colours and [style your shapes](/doc/faq/shape-styles.html) and [connectors](/doc/faq/connector-styles.html) via the _Style_ tab.
   * The style palette at the top of the _Style_ tab changes both the fill and outline colour. Click the left or right arrows to view more styles.
   <br /><img src="/assets/img/blog/basic-flow-style-palette.png" style="width=100%;max-width:200px;height:auto;" alt="Set a new shape or connector style easily with the style palette in draw.io">
   * To set your own colour, click on the colour button next to _Fill_ or _Line_, select a new colour or enter a hex colour code in the top text field. 
   <br /><img src="/assets/img/blog/colour-picker.png" style="width=100%;max-width:200px;height:auto;" alt="Choose a colour from the default or larger colour palette, or enter your own hex colour code">
   <br />**Tip:** Learn about [adaptive colours](/blog/adaptive-colours.html) and [diagramming in dark mode](/blog/dark-mode-diagrams.html).
   * Style a selected connector to have [arrows on both ends](/doc/faq/connector-bidirectional.html) or [no arrows](/doc/faq/connector-no-arrows.html).
   <br /><img src="/assets/img/blog/basic-flow-connector-arrows.png" style="width=100%;max-width:200px;height:auto;" alt="Select an arrow or another connector end style at both the target and source shape in draw.io">
3. [Change the text style](/doc/faq/text-styles.html) of labels on the _Text_ tab.
   * Select a different _Font_ from the list.
   * Add _Bold_, _Italics_, or _Underline_.
   * Change the justification to be left, right or centred.
   * Click on the colour button next to _Font Color_.
   <br /><img src="/assets/img/blog/basic-flow-text-tab.png" style="width=100%;max-width:200px;height:auto;" alt="Style label text via the Text tab in the format panel in draw.io">   

**Tip:** When you edit the text itself, you will see additional HTML formatting - add a numbered or bulleted list, indent your text, use superscript or subscript text and more.

<br />
## Export and share your flow chart

You can share your diagram in a number of different ways via the _File > Export as_ menu. The most common export formats are as images or as a URL.

* Export as a _PNG_, _JPEG_ or _SVG_ to convert your diagram to an image that you can paste into a website or email.
<br /><img src="/assets/img/blog/basic-flow-export-as-png.png" style="width=100%;max-width:300px;height:auto;" alt="Export your diagram as an image to share it in an email or publish it on a webpage or in a document"> &nbsp;&nbsp;&nbsp; <img src="/assets/img/blog/basic-flow.png" style="width=100%;max-width:200px;height:auto;" alt="The diagram exported as a PNG image">
* [Export as a _URL_](/blog/export-url.html) to encode your entire diagram in a URL. When you share this (very long) URL, the person viewing the diagram will see a copy - they don't open or edit your original diagram.

<img src="/assets/img/blog/basic-flow-export-as-url.gif" style="max-width:100%;height:auto;" alt="Encode your diagram in a URL in draw.io to share it easily">
