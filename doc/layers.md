---
title: Work with layers in draw.io
layout: page
faq: true
categories: [Features]
---

图层为图表添加结构和组织。当您与复杂图表交互时，显示或隐藏其各个图层，您可以更轻松地理解它们。

**注意：** 每个形状或连接线（或组）只能放置在一个图层上 - 它不能属于多个图层。

## 在图表中使用图层

以下部分说明如何在 draw.io 中使用图层。

- [Using layers in diagrams](#using-layers-in-diagrams)
  - [Open the Layers dialog](#open-the-layers-dialog)
  - [Add a new layer](#add-a-new-layer)
  - [Rename a layer](#rename-a-layer)
  - [Remove a layer](#remove-a-layer)
- [Work with shapes on layers](#work-with-shapes-on-layers)
  - [Add shapes to a layer](#add-shapes-to-a-layer)
  - [See which layer a shape belongs to](#see-which-layer-a-shape-belongs-to)
  - [Move shapes to another layer](#move-shapes-to-another-layer)
  - [Rearrange layers to move shapes forward or backward](#rearrange-layers-to-move-shapes-forward-or-backward)
- [Hide or display layers](#hide-or-display-layers)
- [Lock layers to prevent changes](#lock-layers-to-prevent-changes)
- [Diagrams that work well with layers](#diagrams-that-work-well-with-layers)


**提示：** [在 draw.io 编辑器中打开示例 gitflow](https://app.diagrams.net/?lightbox=0&highlight=0000ff&edit=_blank&layers=1&page=0&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fgitflow-layers.drawio) - 使用以下部分了解如何在图表中使用这些图层。 

### Open the Layers dialog

Select _View > Layers_ or press ``Ctrl+Shift+L`` / ``Cmd+Shift+L`` to display or hide the _Layers_ dialog.

<img src="/assets/img/blog/view-layers.png" style="max-width:100%;height:auto;" alt="Select View > Layers to open the Layers dialog">

By default, a new diagram has a single _Background_ layer, to which all shapes, connectors and text are added.

From the Layers dialog, you can add new layers and rename them, select which layer to add new shapes to, remove existing layers, and move selected shapes to a layer. 

You can also display and hide layers, which will display or hide all of the shapes, connectors and text that are on those layers. 

Finally, locking a layer makes sure you can't make any inadvertent changes.

### Add a new layer 

At the bottom of the _Layers_ dialog, click on _Add Layer_ (``+``). 

Your new layer will be automatically selected (with a blue background), and any new shapes you add to the drawing canvas will be placed on your new layer.

<img src="/assets/img/blog/layer-add.png" style="max-width:100%;height:auto;" alt="Click on Add Layer (+) in the Layers dialog to add a new layer">

**Duplicate a layer:** Select the layer you want to duplicate, then click on _Duplicate_ in the _Layers_ dialog (a pair of overlapping boxes).

<img src="/assets/img/blog/layer-duplicate.png" style="width=100%;max-width:200px;height:auto;" alt="Select a layer then click on Duplicate (overlapping box) in the Layers dialog to duplicate it">

[_Back to top_](#using-layers-in-diagrams)

### Rename a layer

When you add a new layer, it will be given a default name. Start typing immediately to change its name to something meaningful. You can double click on any layer to edit its new name at any time. 

<img src="/assets/img/blog/layer-rename.png" style="width=100%;max-width:400px;height:auto;" alt="Double click on a layer, and enter a new name">

**Rename a layer via its metadata**

Layers have metadata, just like shapes have metadata. This metadata allowed advanced functionality within your You can also change a layer's name via the _Edit Data_ dialog.

[See how to use metadata and placeholders in labels and tooltips](/blog/placeholders.html)

1. Select a layer, then click on the _Edit Data_ in the _Layers_ dialog (three vertical dots). 
<br /><img src="/assets/img/blog/layer-edit-data.png" style="width=100%;max-width:200px;height:auto;" alt="Select a layer in the Layers dialog, then click on Edit Data">
1. Change the text in the _Label_ field and click _Apply_ to change the layer's name.
<br /><img src="/assets/img/blog/layer-edit-data-dialog.png" style="width=100%;max-width:300px;height:auto;" alt="In the Edit Data dialog for that layer, change the label text and click Apply to rename it">

[_Back to top_](#using-layers-in-diagrams)

### Remove a layer

Remove a layer will delete all of the shapes and connectors that are on it as well as the layer itself. Click on a layer to select it, then click on _Remove_ in the bottom left of the _Layers_ dialog (rubbish bin) to remove the layer and its shapes.

<img src="/assets/img/blog/layer-remove.png" style="width=100%;max-width:250px;height:auto;" alt="Select a layer, then click on the rubbish bin icon to remove it and all of the shapes/connectors it contains">

**Note:** Your diagram must have at least one layer for shapes and connectors to be placed. If there is only one layer in your diagram, you can not delete it. 

[_Back to top_](#using-layers-in-diagrams)

## 在图层上使用形状

形状按照您将它们添加到绘图画布的顺序排列，在您添加它们的图层内。

图层从前往后排列，就像它们在_图层_对话框中从上到下排序一样。放置在较高图层上的形状和连接线不能回到较低图层上的形状后面 - 它们只能在_其图层内_从前往后排列。

### 向图层添加形状

1. 在进行更改之前，请确保图层可见且已解锁（单击眼睛以显示隐藏的图层，单击图层名称左侧的锁定图标）。图层默认已解锁。
2. 在_图层_对话框中选择要添加形状的图层，然后将形状添加到绘图画布。 

<img src="/assets/img/blog/layer-add-shape.gif" style="max-width:100%;height:auto;" alt="Make the layer you want to add the shape or connector to visible and unlocked, then select it, and add your shape/connector">

[_Back to top_](#using-layers-in-diagrams)

### See which layer a shape belongs to

Select one shape or more shapes - make sure they are all on the same layer. Note the dot to the right of the layer name - this shows that your selected shape(s) are on that layer. 

<img src="/assets/img/blog/shape-find-layer.png" style="max-width:100%;height:auto;" alt="Select a shape, note the dot on the right of the layer name - this is the layer the shape belongs to">

**Note:** If you have selected shapes on different layers, you will not see a dot in the Layers dialog.

[_Back to top_](#using-layers-in-diagrams)

### Move shapes to another layer

1. Select the shapes, connectors and text you want to move to another layer. 
2. In the layers dialog, click on the three vertical dots icon to open the list of layer targets, then select the layer you want to move your selected shapes to.

<img src="/assets/img/blog/shapes-move-layers.png" style="max-width:100%;height:auto;" alt="Move the selected shapes to another layer via the Layers dialog">

The dot indicating on which layer your selected shapes are will be updated to your choice.

[_Back to top_](#using-layers-in-diagrams)

### Rearrange layers to move shapes forward or backward

To move one layer's shapes in front of another, you need to change the order of the layers in the _Layers_ dialog. Layers are arranged from top to bottom (front to back on the drawing canvas).

[Learn how the z-order of shapes positions them in front of or behind other shapes](/blog/move-shapes-forwards-backwards.html)

Click and drag a layer in the _Layers_ dialog to place its shapes in front of or behind another layer.

<img src="/assets/img/blog/layer-rearrange.gif" style="max-width:100%;height:auto;" alt="In the Layers dialog, drag a layer higher or lower to move its contents above or below shapes and connectors on the other layers">

**Note:** When you move shapes to a layer, they are placed in front of any existing shapes on that layer, just like when you add new shapes to a layer.

[_Back to top_](#using-layers-in-diagrams)

## Hide or display layers

To understand complex diagrams that use layers, you can display and hide layers. 

In the _Layers_ dialog, click on the eye on the left of layer's name to display or hide the layer.

<img src="/assets/img/blog/layers-display-hide.gif" style="max-width:100%;height:auto;" alt="Click on the eye next to the layer name to display or hide the shapes and connectors on that layer">

**Hide or display layers in the diagram viewer:** Click on the _Layers_ tool at the bottom of the diagram viewer, then click on the eye icons next to the layer names to hide or display the layers. This tool is not available if the diagram only has one layer.

<img src="/assets/img/blog/layers-viewer-display-hide.png" style="max-width:100%;height:auto;" alt="Click on the layer tool then on the eyes next to layer names to hide or display them in the diagram viewer">

**Tip:** [Use custom links to make your diagram interactive](/blog/interactive-diagram-layers.html) and toggle layers on and off when you click on a shape within the diagram. 

[_Back to top_](#using-layers-in-diagrams)

## 锁定图层以防止更改

锁定图层意味着您无法对其进行任何更改 - 您无法添加、移动、编辑、设置样式或删除放置在该图层上的形状和连接线。

在_图层_对话框中，单击要锁定的图层名称左侧的挂锁图标。

<img src="/assets/img/blog/layer-locked-add-shape-failure.gif" style="max-width:100%;height:auto;" alt="Click on the padlock next to a layer's name in the Layers dialog to lock or unlock the layer">

[_Back to top_](#using-layers-in-diagrams)

## 适合使用图层的图表

* [平面图](/blog/floorplans.html) - 在单独的图层上添加家具、电器或 IT 设备、固定装置和装饰。
* [网络图](/blog/network-diagrams.html) - 将防火墙后面的区域或不同子网上的区域放置在不同的图层上。 
* [Gitflow 图](/blog/gitflow-diagram.html) - 将团队或功能分支分离到它们自己的图层上。在灯箱查看器中打开这个[带图层的示例 gitflow 图](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&page=0&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fgitflow-layers.drawio)。