---
title: Using draw.io in Jira Cloud
layout: page
faq: true
categories: [Jira Cloud]
---

draw.io 是一个功能齐全的图表工具，具有大型形状库和各种图表的模板。

**Jira 管理员：** 在可以将任何图表添加到 Jira 问题之前，管理员必须在 Jira Cloud 实例中安装 draw.io 应用。跳转到下面的[管理部分](#administration-and-licensing)。

**Jira 用户：** 如果您是_图表绘制新手_，请先[了解 draw.io 编辑器的布局](/doc/getting-started-editor.html)，然后[创建简单流程图](/doc/getting-started-basic-flow-chart.html)以学习图表绘制的基础知识。

<img src="/assets/img/blog/jira-cloud-drawio-editor.png" style="max-width:100%;height:auto;" alt="Draw diagrams and attach them to Jira Cloud issues with the draw.io app">

## 开始使用

使用 draw.io for Jira Cloud 应用，您可以通过四种不同的方式在问题中嵌入图表。

我们建议您[从 Confluence Cloud 实例嵌入图表](/blog/confluence-diagrams-in-jira.html)以利用实时协作工具、[数据安全](/blog/data-governance-lockdown.html)、[自定义](/doc/faq/drawio-confluence-cloud.html)、[批量导入](/doc/faq/mass-import-gliffy-confluence-cloud.html)、[图表搜索](/blog/confluence-diagram-search.html)和版本控制功能。

替代方案：
* 将图表文件存储在问题本身中（如下）
* [从 Google Drive 嵌入图表](/doc/faq/embed-diagram-googledrive-jira-cloud.html)
* [从 OneDrive 嵌入图表](/doc/faq/embed-diagram-onedrive-jira-cloud.html)

您对嵌入图表文件所做的任何更改都会自动更新其嵌入的任何 Jira Cloud 问题上的图表。

要将图表文件直接附加到 Jira Cloud 问题，请按照下面部分的步骤操作。

### Attach a new diagram to a Jira Cloud issue

1. Click on the _Actions_ in the top right of an issue and select __Add draw.io diagram_.
<br /><img src="/assets/img/blog/jira-cloud-add-diagram.png" style="max-width:100%;height:auto;" alt="Add a draw.io diagram to a Jira Cloud issue">
2. Create your diagram in the draw.io editor. When you save your diagram, you'll be prompted to provide a filename.

Your diagram will be added as a file attached to the issue.
<br /><img src="/assets/img/blog/jira-cloud-attached-diagram.png" style="max-width:100%;height:auto;" alt="Your draw.io diagram file is added as an attachment to the Jira Cloud issue">


### See the draw.io diagrams on a Jira issue

By default, the draw.io Diagrams section is not displayed in Jira issues to keep them as uncluttered as possible.

* Click on the draw.io icon directly above the issue description to display the draw.io Diagrams section.
<br /><img src="/assets/img/blog/jira-cloud-display-drawio-section.png" style="max-width:100%;height:auto;" alt="Display the draw.io diagrams section in your Jira Cloud issue">

**Tip:** draw.io diagram thumbnails in a Jira issue will automatically change colours to match the user's [Jira Cloud theme settings - either dark or light](/blog/dark-theme-drawio-jira.html). If you want the diagram to always display on a specific coloured background, [set a background colour](/blog/dark-theme-drawio-jira.html#set-a-background-colour-in-a-diagram) in the draw.io editor.
<br /><img src="/assets/img/blog/jira-cloud-set-background-colour.png" style="width=100%;max-width:300px;height:auto;" alt="Adding a diagram background ensures your diagram looks the same in both Jira's light and dark themes">

### View a diagram

* Click on the thumbnail in the draw.io Diagrams section in the Jira issue to open it in the lightbox viewer.
* Hover over the diagram to see the viewer toolbar. 
   * Zoom in and out, print or export the diagram from this toolbar.
   * If the diagram has them, step through diagram pages and select the layers to display.
* Click on the cross or the tick in the top right to return to the Jira issue.
<br /><img src="/assets/img/blog/jira-cloud-view-diagram.png" style="width=100%;max-width:400px;height:auto;" alt="View a draw.io diagram attached to a Jira Cloud issue in the lightbox viewer">

### Edit a diagram attached to a Jira issue
* Hover over the thumbnail in the draw.io Diagrams section in the Jira issue and click on the pencil icon to edit the diagram.
<br /><img src="/assets/img/blog/jira-cloud-edit-diagram.png" style="max-width:100%;height:auto;" alt="Edit the draw.io diagram attached to a Jira Cloud issue">


### Delete a diagram from a Jira issue
* Hover over the thumbnail in the draw.io Diagrams section in the Jira issue and click on the trash can icon (delete).
<br /><img src="/assets/img/blog/jira-cloud-delete-diagram.png" style="max-width:100%;height:auto;" alt="Delete a draw.io diagram attached to a Jira Cloud issue">

### Export or print a diagram from a Jira issue

**From within the draw.io editor**
1. Select _File > Export as_ and select the format you want to export the diagram as. 
2. Choose the export options that apply. These will depend on what format you export to. For example, exporting to a PNG image:
<br /><img src="/assets/img/blog/export-png-options.png" style="width=100%;max-width:200px;height:auto;" alt="Choose the export settings for the PNG image">

[Learn more about exporting diagrams](/doc/faq/export-diagram.html)

**From the lightbox viewer**

**Note:** Image files generated from the lightbox viewer do not include the diagram data, unlike if you export to a PNG file from within the draw.io editor.

1. Click on the diagram attached to the Jira issue to open it in the lightroom viewer.
2. Use the toolbar to view the diagram page and select the layers you want to include.
<br /><img src="/assets/img/blog/jira-cloud-view-page-layers.png" style="width=100%;max-width:400px;height:auto;" alt="Select which layers to see in the draw.io lightbox viewer toolbar">
3. Click on the _Export_ tool (camera) to generate a PNG image thumbnail, or _Print_ to print the diagram.
4. Right-click on the generated PNG thumbnail and download it. Left-click on the thumbnail to open the image in a new browser tab. 
<br /><img src="/assets/img/blog/jira-cloud-viewer-export.png" style="width=100%;max-width:400px;height:auto;" alt="Export the draw.io diagram from the lightbox viewer in Jira Cloud">

## Administration and licensing

* [Install the draw.io for Jira Cloud app in your instance via the Atlassian Marketplace](https://marketplace.atlassian.com/apps/1211413/draw-io-diagrams-for-jira?hosting=cloud&tab=overview)
* [Open the app management pages in Confluence and Jira Cloud](/doc/faq/app-management-pages-confluence-jira-cloud.html)
* [Data storage and flow of user data in draw.io for Confluence and Jira Cloud](/doc/faq/data-flow-confluence-jira-cloud.html)
* [Check access rights for draw.io in Jira Cloud](/doc/faq/jira-cloud-insufficient-access-rights.html)
* [Migrate draw.io from Jira Server or DC to Jira Cloud](/doc/faq/migrate-drawio-jira.html)

**Security and Licensing**

* [draw.io is an Atlassian Cloud Fortified app](/blog/drawio-atlassian-cloud-fortified.html)
* [Advantages of a bring-your-own-storage model](/blog/secure-diagramming-storage.html)
* [Get a community draw.io license for Confluence or Jira Cloud](/doc/faq/drawio-community-license-cloud.html)
* [Find the draw.io app version and SEN in Jira Cloud](/doc/faq/app-version-jira-cloud.html)
* [License draw.io for Confluence and Jira Cloud correctly](/doc/faq/license-drawio-confluence-jira-cloud.html)
* [What happens to diagrams when the draw.io app license for Confluence or Jira Cloud becomes invalid?](/doc/faq/unlicensed-drawio-app-confluence-jira-cloud.html)
