---
title: Change the style of shapes
layout: page
faq: true
categories: [Shapes]
---

使用右侧格式面板的_样式_和_文本_选项卡自定义绘图画布上形状或形状组的外观。当您选择一个或多个形状时，draw.io 编辑器会自动切换到形状样式面板。

原始形状样式使用黑色轮廓和纯白色填充颜色。

您可以通过多种方式自定义形状样式 - 单击下面的链接查看如何操作。

- [Use the style palette to change colours](#use-the-style-palette-to-change-colours)
- [Change the fill colour or add a gradient](#change-the-fill-colour-or-add-a-gradient)
  - [Additional fill options and effects](#additional-fill-options-and-effects)
- [Change the shape outline](#change-the-shape-outline)
- [Change the opacity of the shape](#change-the-opacity-of-the-shape)
- [Apply effects to shapes](#apply-effects-to-shapes)
- [Copy and paste styles](#copy-and-paste-styles)
- [Set a default style](#set-a-default-style)
- [Edit the shape style and behaviour](#edit-the-shape-style-and-behaviour)
  - [Edit shape properties in the Style tab](#edit-shape-properties-in-the-style-tab)
  - [Edit the XML that defines the shape properties](#edit-the-xml-that-defines-the-shape-properties)
- [Related features](#related-features)

在设置任何内容的样式之前，您必须选择它。单击形状以选择它，或按住 ``Shift`` 并单击多个形状以选择多个。

您看到的样式选项将取决于您选择的形状。例如，圆形或椭圆形没有角，因此_圆角_选项将不可用。

**上下文相关的形状样式：** 设置形状样式后，要以相同样式添加新形状并将其连接到该形状，请将鼠标悬停在现有形状上并单击其中一个方向箭头。 

## Use the style palette to change colours

The style palette at the top of the _Style_ tab changes both the fill and outline colour. 

Click the left or right arrows or click on the page dots underneath the palette to view more styles.
<br /><img src="/assets/img/blog/basic-flow-style-palette.png" style="width=100%;max-width:200px;height:auto;" alt="Set a new shape or connector style easily with the style palette in draw.io">

If you are diagramming in [dark mode](/blog/dark-mode-diagrams.html), you'll see both a triangle for the light mode colour in the bottom right and the adapted colour for dark mode on top. By default, the editor [automatically adapts the colours](/blog/adaptive-colours.html) when you change to light or dark mode.
<br /><img src="/assets/img/blog/basic-flow-style-palette-dark.png" style="width=100%;max-width:200px;height:auto;" alt="Set a new shape or connector style easily with the style palette in draw.io">


## Change the fill colour or add a gradient

1. Click on the colour button next to _Fill_ to see the colour palette.
<br /><img src="/assets/img/blog/style-tab-fill-colour.png" style="width=100%;max-width:400px;height:auto;" alt="Click on the Fill colour button to set a new shape fill colour"> <img src="/assets/img/blog/colour-picker.png" style="width=100%;max-width:150px;height:auto;" alt="Select a new fill colour from the colour palette">
2. Choose a new colour from the palette, or enter a colour's precise hex code in the text box (without the leading ``#``), then click _Apply_.

### Additional fill options and effects

<img src="/assets/img/blog/shape-fill-options.png" style="width=100%;max-width:300px;height:auto;" alt="Change the fill style options to change the background in the selected shapes">

**Gradient:** Click the _Gradient_ checkbox, select the direction in which you want the fill colour to change from the drop-down, and click on the colour button to select a new gradient colour from the colour palette.

**Transparent:** Deselect the _Fill_ checkbox to remove the fill colour and make the background of the shape transparent.

**Glass effect:** Select the _Glass_ checkbox to add a gradient to the fill and outline so that it looks like a reflective surface. You can have both a gradient and the glass effect enabled at the same time. 

**Lane colour:** To add a fill colour to background of swimlanes, select the lane, then enable the _Lanecolour_ checkbox. You can apply both a gradient and the glass effect to the swimlane background too.
<br /><img src="/assets/img/blog/style-tab-lanecolor.png" style="width=100%;max-width:400px;height:auto;" alt="Change the fill colour of a swimlane by clicking on Lanecolor in the Style tab of the format panel">

## Change the shape outline

1. Click on the _Line_ colour button, and select a new colour from the palette.
2. Select a new line style for the outline of a shape from the drop down list. Choose between solid, dashed, and three patterns of dotted. 
3. Enter a new value in the textbox next to the outline pattern to make the line thicker. The default is ``1pt``.
<br /><img src="/assets/img/blog/style-tab-line-options.png" style="width=100%;max-width:300px;height:auto;" alt="Change the style of the shape outline to use a different pattern, colour, or thickness">

**No outline:** Click on the _Line_ checkbox and disable the outline. 

**Add space around the shape:** Enter a new value in the _Perimeter_ checkbox to add space between the outline of the shape, and it's actual size. This will move the connection points and the outer edge that connectors connect to outwards, away from the outline of the shape.
<br /><img src="/assets/img/blog/style-tab-perimeter.png" style="width=100%;max-width:300px;height:auto;" alt="Increase the Perimeter in the Style tab to move connection points and the floating border to which connectors attach away from the shape">

## 更改形状的不透明度

您可以使形状更加透明，以便其下方的任何形状都能显示出来。

在_不透明度_文本字段中输入新值，或使用向上/向下箭头更改其值。 
<br /><img src="/assets/img/blog/shape-opacity.png" style="width=100%;max-width:300px;height:auto;" alt="Set a new value for Opacity to make a shape more transparent and let shapes underneath show through">

## Apply effects to shapes

**Round sharp corners:** Click on the _Rounded_ checkbox to round all the corners of any sharp-cornered basic shape. 
<br /><img src="/assets/img/blog/style-tab-rounded.png" style="width=100%;max-width:300px;height:auto;" alt="Select the Rounded checkbox in the Style tab to round sharp corners of shapes">

**Add a shadow:** Click on the _Shadow_ checkbox to add a drop shadow to all shapes. Shadows can also be applied to connectors. 
<br /><img src="/assets/img/blog/style-tab-shape-shadow.png" style="width=100%;max-width:300px;height:auto;" alt="Click the Shadow checkbox to add a shadow to selected shapes and connectors">

**Apply the rough sketch style:** To make the shapes appear as if they are hand drawn, click the _Sketch_ checkbox. Additional style options for the rough style are available in the style _Properties_. 
<br/>[See how to use the rough sketch style and change the sketch style properties](/blog/rough-style.html)
<br /><img src="/assets/img/blog/style-tab-shape-sketch.png" style="width=100%;max-width:300px;height:auto;" alt="Click the Sketch checkbox to make the selected shapes and connectors appear roughly hand drawn">

## 复制和粘贴样式

1. 选择要复制样式的形状。
2. 在格式面板的_样式_选项卡中，单击_复制样式_。
3. 选择要应用此样式的其他形状或连接线。在_样式_选项卡中，单击_粘贴样式_。
<br /><img src="/assets/img/blog/styles-copy-paste.gif" style="width=100%;max-width:300px;height:auto;" alt="Copy and paste styles from one shape or connector to another in draw.io">

## Set a default style

When you set a new default style, any new shape you place on the drawing canvas from the shape libraries, the toolbar (in modern mode) and the double-click shape selection box will use the new default style. 

1. Select the shape that has the style you want to use as the new default. 
2. Click _Set as Default Style_ in the _Style_ tab of the format panel. 
3. Hover over shapes in the shape libraries on the left to see a preview of them using the new default style.
<br /><img src="/assets/img/blog/style-tab-default-style.png" style="width=100%;max-width:500px;height:auto;" alt="Set a new default style for all shapes in the Style tab of the format panel">

**Clear the default style:** Make sure nothing is selected so you can see the _Diagram_ tab in the format panel, then click _Clear Default Style_.
<br /><img src="/assets/img/blog/diagram-tab-clear-default-style.png" style="width=100%;max-width:150px;height:auto;" alt="Clear the default style using the button on the Diagram tab when nothing is selected in your diagram">

This will clear the default styles for both shapes and connectors.

[Learn more about the global diagram options](/doc/faq/diagram-options.html)

## Edit the shape style and behaviour

Other than using the basic options in the _Style_ tab, you can edit a shape's style properties in two ways.

### Edit shape properties in the Style tab

1. With a shape selected, expand the _Property_ section at the bottom of the _Style_ tab in the format panel. 
2. Change the _Value_ of the shape properties to change additional style options and how the shape behaves. 
<br /><img src="/assets/img/blog/shape-properties.png" style="width=100%;max-width:300px;height:auto;" alt="Expand the Properties at the bottom of the Style tab to set additional style options on shapes and connectors">

**Note:** Only those properties that can be applied to the selected shape will be available in this property list. 

### 编辑定义形状属性的 XML

如果您知道要设置的形状属性名称和值，直接编辑形状的 XML 描述文本可能会更快。

例如，一个具有粗糙草图样式的矩形，其圆角使用自定义弧大小、自定义周长大小和不透明的轮廓，其形状样式如下所示：
   ```
   rounded=1;whiteSpace=wrap;html=1;sketch=1;fillColor=#dae8fc;
   strokeColor=#6c8ebf;perimeterSpacing=5;arcSize=24;
   strokeOpacity=59;
   ```
**编辑形状样式**

1. 右键单击形状，然后从上下文菜单中选择_编辑样式_。或者，选择形状后，在 Windows 上按 ``Ctrl+E``，在 macOS 上按 ``Cmd+E``。
2. 使用 property=value 对编辑 XML 描述以描述您希望该形状使用的形状样式，然后单击_应用_。
<br /><img src="/assets/img/blog/edit-style-dialog.png" style="width=100%;max-width:300px;height:auto;" alt="Edit the XML description of a shape to define its style and behaviour">

## 相关功能

* [使用快捷键更快地设置形状样式](/blog/shortcut-styles.html)
* [了解如何更改文本标签和文本形状的样式](/doc/faq/text-styles.html)
* [更改连接线的样式](/doc/faq/connector-styles.html)
* [创建您自己的自定义形状](/doc/faq/shape-complex-create-edit.html)
* [在 draw.io for Confluence Cloud 中设置自定义默认样式](/doc/faq/custom-styles-confluence-cloud.html)