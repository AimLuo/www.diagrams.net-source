---
title: Use the draw.io editor
layout: page
categories: [features]
---

draw.io 是一个免费的开源图表应用，您可以在线在 [app.diagrams.net](https://app.diagrams.net) 使用，也可以离线使用（draw.io 桌面版）。

作为面向团队的安全优先图表应用，我们提供图表功能，您可以选择在哪里保存图表数据。有许多不同的[与其他平台和应用程序的集成](/integrations.html)，包括 [Atlassian Confluence Cloud](/doc/drawio-confluence-cloud.html)、Google Workspace 和 Classroom、GitHub、Gitlab、Notion、Microsoft Office 365。

无论您在哪里使用它，我们的 draw.io 图表编辑器看起来都一样，并提供相同的主要功能。您可以在一个集成中打开在另一个集成中创建的图表。

[<img src="/assets/img/blog/tutorial-menu-header.png" style="width=100%;max-width:85px;" alt="The draw.io menu">](#menu)[<img src="/assets/img/blog/tutorial-toolbar-header.png" style="width=100%;max-width:98px;" alt="The draw.io toolbar">](#toolbar)[<img src="/assets/img/blog/tutorial-shapes-header.png" style="width=100%;max-width:154px;" alt="Shapes and shape libraries in draw.io">](#shapes-and-shape-libraries)[<img src="/assets/img/blog/tutorial-canvas-header.png" style="width=100%;max-width:154px;" alt="The draw.io drawing canvas">](#drawing-canvas)[<img src="/assets/img/blog/tutorial-format-header.png" style="width=100%;max-width:154px;" alt="The format panel in draw.io">](#format-panel)

## draw.io 编辑器

与大多数图表应用一样，您在工具栏和绘图画布周围的面板中看到的项目是上下文相关的。将根据您在绘图画布上选择的元素类型显示工具和选项。

如果您以前使用过图表工具，您会熟悉图表编辑器的布局。

**提示：** 将鼠标悬停在 draw.io 编辑器中的任何按钮、工具或选项上，以查看说明其用途的工具提示。

<img src="/assets/img/blog/interface-introduction.png" style="max-width:100%;height:auto;" alt="The draw.io editor, its tools and panels">

以下部分涵盖了所有主要的 draw.io 编辑器功能。

- [The draw.io editor](#the-drawio-editor)
  - [Menu](#menu)
  - [Toolbar](#toolbar)
  - [Shapes and shape libraries](#shapes-and-shape-libraries)
    - [Enable/disable shape libraries](#enabledisable-shape-libraries)
    - [Scratchpad](#scratchpad)
    - [Search shapes](#search-shapes)
  - [Drawing canvas](#drawing-canvas)
    - [Page tabs](#page-tabs)
  - [Format panel](#format-panel)
    - [Style tab](#style-tab)
    - [Text tab](#text-tab)
    - [Arrange tab](#arrange-tab)
    - [Global diagram options](#global-diagram-options)
- [Keyboard shortcuts](#keyboard-shortcuts)
- [Next step: Draw a diagram](#next-step-draw-a-diagram)

### 菜单

draw.io 中的菜单与其他应用程序的工作方式相同。功能按以下菜单排列。

根据您在图表中选择的内容，某些菜单项将不可选择。例如，如果您没有选择形状，则无法编辑形状的样式。

* **文件** - 处理图表文件（新建、打开、导入/导出和打印），以及打开或自定义创建形状库。
* **编辑** - 选择和编辑图表中的形状和连接线及其样式。
* **视图** - 隐藏或显示 draw.io 编辑器中的各种面板和辅助工具，包括便笺本、图层、标尺等。
* **排列** - 分组和组织形状和连接线，[插入模板和图像](/doc/faq/arrange-insert-menu.html)，使用自动布局功能。
* **附加** - 启用不同的编辑器主题，使用数学排版，启用/禁用开始屏幕和自动保存，以及使用标签或添加自定义配置。
* **帮助** - 查看键盘快捷键，查看支持信息或下载 draw.io 的桌面版本。

**提示：** 菜单右侧是状态消息，显示是否有未保存的编辑或图表是否已自动保存。

[_Back to top_](#the-drawio-editor)

### 工具栏

工具栏中的某些工具需要在图表中选择正确的元素。例如，如果您没有选择形状、连接线或文本，_删除_工具将显示为浅灰色且不可用。

<img src="/assets/img/blog/toolbar.png" style="max-width:100%;height:auto;" alt="The draw.io toolbar">

从左到右依次为：
* **视图** _(三个面板)_ - 隐藏或显示格式面板，或图层和轮廓对话框。
* **缩放** _(数字百分比)_ - 使图表在编辑器中显示得更大或更小。这不会影响图表的导出或打印大小。
* **放大/缩小** _(放大镜)_ - 放大或缩小图表。
* **撤销/重做** _(弯曲箭头)_ - 撤销或重做您的更改。
* **删除** _(垃圾桶)_ - 删除选定的形状。
* **置于顶层/置于底层** _(分层形状)_ - 将选定的形状移动到图表的前面或后面，将它们排列在未选定形状的上方或下方。
* **填充颜色** _(油漆桶)_ - 更改选定形状的填充颜色。
* **线条颜色** _(笔和线条)_ - 更改选定形状的轮廓或连接线的颜色。
* **阴影** _(带阴影的框)_ - 启用或禁用选定形状上的阴影。
* **连接** _(箭头)_ - 从下拉列表中选择连接线样式并应用于选定的连接线。
* **路径点** _(带两个连接点的线条)_ - 选择路由样式以更改选定连接线在绘图画布上的弯曲方式。
* **插入** _(加号)_ - 插入常用形状、手绘图形、图像、模板、布局等。
* **表格** _(网格)_ - 单击然后拖动或单击表格中的某个点以插入具有选定行和列的表格形状。

工具栏右端有三个视图选项：
* **全屏** _(框和角)_ - 关闭左右面板，使绘图画布占据 draw.io 窗口的完整大小。
* **格式面板** _(两个面板)_ - 显示或隐藏右侧的格式面板。
* **折叠/展开** _(向上箭头)_ - 显示或隐藏文件名和 draw.io 应用程序图标。

[_Back to top_](#the-drawio-editor)

### 形状和形状库

形状被组织成逻辑组，称为形状库。由于形状库太多，不会同时显示所有形状库。

**提示：** 通过单击名称来展开或折叠左侧面板中的每个形状库。

<img src="/assets/img/blog/shape-library-panel.png" style="width=100%;max-width:300px;height:auto;" alt="Shapes are arranged into logical groups called shape libraries in draw.io">

[_Back to top_](#the-drawio-editor)

#### 启用/禁用形状库

为了更轻松地创建图表，仅启用您正在处理的特定图表所需的形状库。

1. 单击左侧面板底部的_更多形状_。
2. 滚动浏览各种形状库 - 这些形状库按有用的类别排列，适用于不同类型的图表。单击形状库名称旁边的复选框以启用或禁用它。
<br /><img src="/assets/img/blog/shape-library-dialog.png" style="width=100%;max-width:300px;height:auto;" alt="Select the shape libraries you want to work with in draw.io">
3. 单击_应用_。

[See how to add shapes to the drawing canvas](#add-shapes-to-the-drawing-canvas)  

#### 便笺本

[便笺本是您的个人形状库](/doc/faq/scratchpad.html)，您可以在其中添加最常用的形状或形状组。

1. 将一个或多个选定的形状从绘图画布拖到便笺本上。
2. 单击您已保存到便笺本的形状或形状组之一，将另一个副本添加到绘图画布，就像从形状库中添加形状一样。

<img src="/assets/img/blog/scratchpad-add-multiple-shapes.gif" style="width=100%;max-width:400px;height:auto;" alt="Add multiple shapes as one element on the scratchpad in draw.io">

[_Back to top_](#the-drawio-editor)

#### 搜索形状

有如此多的形状被组织成如此多的库，以至于很难找到它们。在形状搜索字段中输入形状的名称，您将获得多个匹配项。如果您在线，这也会找到匹配的剪贴画形状。

**提示：** 如果找不到您要查找的形状，请尝试搜索相关词。

<img src="/assets/img/blog/search-shapes.png" style="width=100%;max-width:150px;height:auto;" alt="Searching for a pie chart shape for an infographic in draw.io">

[_Back to top_](#the-drawio-editor)

### 绘图画布

通过在编辑器中间的绘图画布上放置、连接和设置形状样式来绘制图表。绘图画布默认显示网格，以帮助您整齐地对齐和间距形状。

* **平移绘图画布** 使用滚动条，或在绘图画布的空白区域右键单击/中键单击并拖动以移动画布。使用鼠标滚轮垂直移动画布。
* **放大和缩小** 使用工具栏中的放大/缩小工具，或在 Windows 上按住 ``Ctrl``，在 macOS 上按住 ``Cmd``，然后使用滚轮放大和缩小绘图画布。这不会更改图表的大小。

**提示：** 通过_视图_菜单启用标尺。

<img src="/assets/img/blog/drawing-canvas.png" style="width=100%;max-width:400px;;height:auto;" alt="The drawing canvas of draw.io">

[Move the drawing canvas on touchscreens and in the outline panel](/doc/faq/drawing-canvas-move)

#### 页面选项卡

将复杂图表组织成多个页面。

* 单击绘图画布下方的 _⋮_（垂直省略号）以访问图表页面菜单。
* 单击页面选项卡以查看该页面。
* 通过单击 _+_（加号）添加新页面。

[了解如何在图表中使用多个页面](/blog/multiple-page-diagrams.html)

[_Back to top_](#the-drawio-editor)

### 格式面板

右侧的格式面板包含您可以更改的选项和属性，以排列和设置形状、连接线、文本和图表的样式。

您看到的内容是上下文相关的。例如，当您单击连接线时，您将看到只能应用于连接线的其他样式选项。如果您只选择文本而不选择形状或连接线，您将只看到文本样式选项。

#### Style tab

When you have selected one or more shapes, you can [change the fill and outline colour of shapes](/doc/faq/shape-styles.html), edit styles, [copy and paste styles](/doc/faq/styles-copy-paste.html) in the Style tab in the format panel on the right. You can [change how a selected connector is drawn](/doc/faq/connector-styles.html) - curved, straight or with sharp right-angles, if it is a broken line or solid, whether line jumps are used and which arrows are used at either end of the connector, and more.

Compare the different style options below when a shape is selected (left) and when a connector is selected (right).

<img src="/assets/img/blog/style-tab-shape.png" style="width=100%;max-width:300px;;height:auto;" alt="The Style tab in the format panel lets you change shape and connector styles in draw.io">  <img src="/assets/img/blog/style-tab-connector.png" style="width=100%;max-width:300px;;height:auto;" alt="The Style tab in the format panel lets you change shape and connector styles in draw.io">

To learn how to work with styles, follow our [basic flow chart tutorial](/doc/getting-started-basic-flow-chart.html).

[_Back to top_](#the-drawio-editor)

#### 文本选项卡

使用右侧格式面板的[_文本_选项卡](/doc/faq/text-styles.html)更改标签的字体、大小和样式。您还可以更改文本的垂直和水平对齐方式、书写方向、字体和背景颜色以及不透明度，并在文本周围添加间距。

默认情况下启用_自动换行_和_格式化文本_。这允许您像 HTML 一样设置标签文本内的字符和单词样式，这也支持超链接。

**提示：** 双击文本以编辑文本并选择标签的一部分。然后，只显示_文本_选项卡（右侧），因为您不是在编辑形状。

Compare the different style options below when a shape is selected (left) and when a connector is selected (right).

<img src="/assets/img/blog/text-tab.png" style="width=100%;max-width:300px;;height:auto;" alt="Style your labels in the Text tab in the format panel on the right in draw.io">  <img src="/assets/img/blog/text-tab-in-label.png" style="width=100%;max-width:300px;;height:auto;" alt="Only the Text tab in the format panel is displayed when you edit the text in a label in draw.io">

[_Back to top_](#the-drawio-editor)

#### 排列选项卡

通过格式面板上的[_排列_选项卡](/doc/faq/arrange-tab.html)更改形状和连接线的位置，将它们发送到前面或后面，更改它们的大小，或旋转它们。

单击_编辑数据_以手动编辑选定形状的元数据，或单击_编辑链接_以添加超链接。

**注意：** 选择连接线时（右）_排列_选项卡显示的选项比选择形状时（左）少。

<img src="/assets/img/blog/arrange-tab-shape.png" style="width=100%;max-width:300px;;height:auto;" alt="Organise your shapes on the drawing canvas with the Arrange tab in the format panel in draw.io">  <img src="/assets/img/blog/arrange-tab-connector.png" style="width=100%;max-width:300px;;height:auto;" alt="Organise your connectors on the drawing canvas with the Arrange tab in the format panel in draw.io">

[_Back to top_](#the-drawio-editor)

#### 全局图表选项

如果您没有选择任何内容，您将看到[适用于整个图表](/doc/faq/diagram-options.html)和绘图画布的选项。

* 在_图表_选项卡中更改打印和绘图画布选项。
* 在_样式_选项卡中向形状、文本和连接线应用新的全局样式。

<img src="/assets/img/blog/diagram-options.png" style="width=100%;max-width:300px;;height:auto;" alt="The page and drawing canvas options available in draw.io">   <img src="/assets/img/blog/diagram-options-style.png" style="width=100%;max-width:300px;;height:auto;" alt="The style options let you globally change the shape, connector and text styles in draw.io">

[_Back to top_](#the-drawio-editor)

## 键盘快捷键

使用以下键盘快捷键可以更高效地使用我们的 draw.io 编辑器。

[<img src="https://app.diagrams.net/shortcuts.svg" style="width=100%;max-width:600px;;height:auto;" alt="The page and drawing canvas options available at app.diagrams.net">](https://app.diagrams.net/shortcuts.svg)
<br />[_查看和打印这些键盘快捷键_](https://app.diagrams.net/shortcuts.svg)

## 下一步：绘制图表

遵循这个[基本流程图教程](/doc/getting-started-basic-flow-chart.html)来创建您的第一个图表。

<img src="/assets/img/blog/basic-flow.png" style="width=100%;max-width:200px;height:auto;" alt="The diagram exported as a PNG image">s