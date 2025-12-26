---
title: Automatically number shapes as you insert them
layout: page
faq: true
categories: [Plugins]
---

**重要：** ``Enumerate`` 形状属性允许您向选定的形状和连接线添加编号标签。默认情况下，它不能应用于添加到绘图画布的任何新形状。

但是，``Enumerate`` 形状属性可以让您控制图表的哪些部分被编号，并且可以自定义以在容器形状或表格单元格内的形状和连接线上工作，这与编号插件不同。

[了解如何使用 ``Enumerate`` 形状属性](/blog/number-shapes.html)

## 改用编号插件

_此插件应按原样使用，作为开发人员的不受支持的示例。_

使用编号插件为图表中的形状添加自动编号。它会在将每个形状添加到图表时为其编号。

您可以通过在格式面板的_排列_选项卡中将形状向前或向后移动来更改顺序 - 编号基于它们在图表中的 z 顺序（深度）。

**注意：** 这不适用于容器形状和表格形状，因为它们是复合形状 - 编号插件将为每个部分编号。请改用 [``Enumerate`` 形状属性](/blog/number-shapes.html)。 

[<img src="/assets/img/blog/number-plugin.gif" style="max-width:100%;height:auto;" alt="The number plugin automatically includes numbers on shapes as you add them to your diagram">](https://app.diagrams.net/?highlight=0000ff&edit=_blank&p=number&layers=1&nav=1&title=number-plugin#R5VdNj5swEP01HCsBJnxcl2bbSu2hiqpWvTkwAVLDIGNC0l9fE0yAJLCs1DTK9hLhNzMZz%2BP5ARrx0%2F0HTvP4C4bANFMP9xp5r5mma3jytwYODbBwSANEPAkbyOiAVfIbFKgrtExCKAaJApGJJB%2BCAWYZBGKAUc6xGqZtkA275jSCC2AVUHaJfk9CESvUsL0u8BGSKFatXdNpAiltk9UkRUxDrHoQWWrE54iiuUr3PrCau5aXpu55JHraGIdMzCl4%2Bunhj8J59hfbT18zd73aftu9I3bzNzvKSjWx2q04tBRAKBlRS%2BQixggzypYd%2BsSxzEKo%2B%2Bhy1eV8RswlaEhwC0Ic1O2lpUAJxSJlKtr0rBuNDqegAksewMRELd2C8gjE1OiL002Q4gVMQfCDLOTAqEh2w51QJaPolNcxLS8U2a8gvt3mFPEdrTVHVZwIWOX0OH0lD9uQwk3CmI8M%2BbGWhBTcTSDxQnD8Bb2IHbiw3pxI3wEXsJ%2Bm%2FZIkVWBaagx1uttl1Tsq7aRx75TY%2Bo1oJe5b03Mj0zl6du6pZ8v8b4m3Rs7IvyG%2B3eakkcSYrsviZRMZOs64dYyZzd%2BwFHtoKYZz6SnuFUtxb2Up1gynfjBlO3Mtxbursp2XiX8APZ89Isn9n5HeDEEzJt%2Bw4TEc4%2Fwl5IpjXGX4dpZhvAXlWvqZE7u3U65cdl9Cx1jvc5Is%2FwA%3D)

[Open this diagram in the viewer](https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&p=number&layers=1&nav=1&title=number-plugin#R5VdNj5swEP01HCsBJnxcl2bbSu2hiqpWvTkwAVLDIGNC0l9fE0yAJLCs1DTK9hLhNzMZz%2BP5ARrx0%2F0HTvP4C4bANFMP9xp5r5mma3jytwYODbBwSANEPAkbyOiAVfIbFKgrtExCKAaJApGJJB%2BCAWYZBGKAUc6xGqZtkA275jSCC2AVUHaJfk9CESvUsL0u8BGSKFatXdNpAiltk9UkRUxDrHoQWWrE54iiuUr3PrCau5aXpu55JHraGIdMzCl4%2Bunhj8J59hfbT18zd73aftu9I3bzNzvKSjWx2q04tBRAKBlRS%2BQixggzypYd%2BsSxzEKo%2B%2Bhy1eV8RswlaEhwC0Ic1O2lpUAJxSJlKtr0rBuNDqegAksewMRELd2C8gjE1OiL002Q4gVMQfCDLOTAqEh2w51QJaPolNcxLS8U2a8gvt3mFPEdrTVHVZwIWOX0OH0lD9uQwk3CmI8M%2BbGWhBTcTSDxQnD8Bb2IHbiw3pxI3wEXsJ%2Bm%2FZIkVWBaagx1uttl1Tsq7aRx75TY%2Bo1oJe5b03Mj0zl6du6pZ8v8b4m3Rs7IvyG%2B3eakkcSYrsviZRMZOs64dYyZzd%2BwFHtoKYZz6SnuFUtxb2Up1gynfjBlO3Mtxbursp2XiX8APZ89Isn9n5HeDEEzJt%2Bw4TEc4%2Fwl5IpjXGX4dpZhvAXlWvqZE7u3U65cdl9Cx1jvc5Is%2FwA%3D)

[More information about draw.io plugins](/doc/faq/plugins.html)

## Load the number plugin

* To create a new diagram in our online editor with the plugin already loaded, go to [https://app.diagrams.net/?splash=0&p=number](https://app.diagrams.net/?splash=0&p=number)

## Permanently load the number plugin

If you want to always use the number plugin, add it to the plugins list so it will be loaded each time you create or edit a diagram.

1. From the menu, select _Extras > Plugins_.
<br /><img src="/assets/img/blog/extras-plugins.png" style="width=100%;max-width:400px;height:auto;" alt="Open the plugins list">
2. Click _Add_.
<br /><img src="/assets/img/blog/add-plugin.png" style="width=100%;max-width:200px;height:auto;" alt="Add a new plugin">
3. Select ``number`` in the drop-down list of built-in plugins, then click _OK_.
<br /><img src="/assets/img/blog/add-number-plugin.png" style="width=100%;max-width:200px;height:auto;" alt="Add the number plugin">
4. Click _Apply_.
<br /><img src="/assets/img/blog/add-number-plugin-apply.png" style="width=100%;max-width:200px;height:auto;" alt="Add the number plugin">

Reload your browser tab to load the plugin into the diagram editor.

## Show or hide the numbering in your diagram

Click _View > Number_ to show or hide the numbering in your diagram.

## Share a diagram using the properties plugin

By default, diagrams published to URLs do not load plugins.

To allow someone to see your diagram with its numbers on shapes, when you publish a diagram to a URL (_File > Publish Link_), add the ``&p=number`` URL parameter to the link before you share it (as highlighted in blue in the screenshot below).

<img src="/assets/img/blog/publish-link-number-plugin.png" style="width=100%;max-width:400px;height:auto;" alt="Share a link to your diagram and enable the number plugin">

**Note:** Plugins work with the web version of draw.io ([app.diagrams.net](https://app.diagrams.net/)) or [our Docker image](/blog/diagrams-docker-app) if you want to run your own server. They do not work with draw.io for Confluence/Jira or with draw.io Desktop.
