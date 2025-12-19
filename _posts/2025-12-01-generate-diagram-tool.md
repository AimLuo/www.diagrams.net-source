---
layout: post
author: draw.io
slug: generate-diagram-tool
date: 2025-12-01 09:24:00
title: Generate more types of diagrams in draw.io with the new sparkle tool
tags: [features]
categories: [features, import, templates]
---

The smart templates feature has been upgraded - click on the new _Generate_ tool (sparkle button) in the draw.io toolbar to generate a diagram. The _Generate_ tool uses multiple AI generators to support a wider range of diagrams, including interface mock-ups, infrastructure diagrams, Mermaid diagrams and more. 
<br /><img src="/assets/img/blog/generate-mockup.png" style="width=100%;max-width:500px;height:auto;" alt="The new generate diagram tool">

**Tips:** 
 * The _Generate_ tool is available in all the [draw.io editor themes](/doc/faq/editor-theme-change.html) that have a toolbar - Classic, Atlas, Simple and Sketch - in the Atlassian draw.io apps and our [online editor](https://app.diagrams.net). 
 * While you can still generate a diagram from within the template library as a [smart template](/blog/smart-diagram-generation.html), you can also edit queries via the Generate tool. 

## Generate a diagram

Make sure you write the type of diagram you want at the start of the query - this is what decides which AI generator is chosen, as each generator is good at only a small subset of diagrams.

1. Open the Generate dialog - click on the sparkle button. 
<br /><img src="/assets/img/blog/generate-sparkle.png" style="width=100%;max-width:200px;height:auto;" alt="Click on the Generate tool in the draw.io toolbar to open the Generate diagram dialog">
2. Describe the diagram you want to generate, then press ``Enter`` or click on _Send_. 
<br /><img src="/assets/img/blog/generate-send.png" style="width=100%;max-width:250px;height:auto;" alt="Write a description of your diagram and send your query in the draw.io Generate tool">
3. Your query will be sent to the AI tools to analyse and generate a preview of a diagram - this may take a little time. If the result doesn't match your query, click _Refresh_ to regenerate a different version - keep in mind that AI tools may not return sensible results.
<br /><img src="/assets/img/blog/generate-refresh.png" style="width=100%;max-width:200px;height:auto;" alt="If your diagram">
4. Click _+_ to add the diagram to the drawing canvas.
<br /><img src="/assets/img/blog/generate-insert.png" style="width=100%;max-width:200px;height:auto;" alt="Insert the generated diagram on the drawing canvas in draw.io">
5. **Online draw.io editor only:** To open the diagram in a new browser tab and new diagram instead of inserting it on the current diagram page click on _Open in New Window_.
<br /><img src="/assets/img/blog/generate-open-new-window.png" style="width=100%;max-width:200px;height:auto;" alt="Open a generated diagram in a new draw.io to generate a new or updated version of the diagram">

The colours in generated diagrams may not be optimised for draw.io's [adaptive colour](/blog/adaptive-colours.html) feature. You may need to tweak shape and diagram styles after inserting the generated diagram on the drawing canvas. In the example below, the generated diagram was much easier to see in [dark mode](/blog/dark-mode-diagram-editor.html). 

<img src="/assets/img/blog/generate-gantt-mermaid.png" style="width=100%;max-width:500px;height:auto;" alt="Edit your diagram generation query in draw.io to generate a new or updated version of the diagram">

Some diagrams, like the Gantt chart above, will be generated in [Mermaid code](/blog/mermaid-diagrams.html) instead of being converted to native draw.io shapes. Hover over the diagram on the drawing canvas to see this Mermaid code, and double click on it to edit it. 
<br /><img src="/assets/img/blog/generate-gantt-mermaid-edit.png" style="width=100%;max-width:300px;height:auto;" alt="Edit the generated mermaid diagram in draw.io">

**Tip:** If you want to the generator to use Mermaid, make sure you write that in your query, either before or directly after the diagram type.

### Preview the generated diagram

While you can hover over the diagram for a small preview, to see a larger preview, click on the _Preview_ magnifying class. 
<br /><img src="/assets/img/blog/generate-hover.png" style="width=100%;max-height:150px;height:auto;" alt="Hover over the generated diagram to see a small preview in draw.io"> &nbsp; <img src="/assets/img/blog/generate-preview.png" style="width=100%;max-height:150px;height:auto;" alt="Click on the Preview tool to see a larger preview of your generated diagram in draw.io">

### Edit your query

1. Click on _Edit_ (pen icon) to paste that query text in the description box. 
2. [Refine the query](/blog/write-query-generate-diagram.html) and click _Send_ to generate an updated diagram. 
<br /><img src="/assets/img/blog/generate-edit-query.png" style="width=100%;max-width:200px;height:auto;" alt="Edit your diagram generation query in draw.io to generate a new or updated version of the diagram">

The edited queries do not overwrite the earlier generated diagrams - you can add any or all of these to the diagram canvas. 
<br /><img src="/assets/img/blog/generate-insert-multiple-diagrams.png" style="width=100%;max-width:500px;height:auto;" alt="You can insert each of the generated diagrams - editing a query does not overwrite the generated example in draw.io">

**Tip:** To copy just the text of your query, click the copy icon next to the pen.

### Delete a query

* Click _Remove_ (rubbish bin) to delete a query from the Generate dialog. 
* To clear the dialog complete, remove all queries. 
<br /><img src="/assets/img/blog/generate-delete-query.png" style="width=100%;max-width:200px;height:auto;" alt="Click on the Remove trash can icon to remove a query from the draw.io generate diagram tool">

## Related

Learn about [when it makes sense to generate diagrams](/blog/generated-diagrams.html) and how to [write better queries](/blog/write-query-generate-diagram.html) for more accurate diagram generation.
  
**For Atlassian administrators:** [enable smart templates in draw.io for Confluence Cloud](/doc/faq/confluence-cloud-enable-smart-templates.html).
  
To disable this feature completely, hide the sparkle button and menu items, set ``"enableAi": false`` in the draw.io app configuration. There are many [diagram generation options](/doc/faq/configuration-custom-ai-actions-endpoints) you can customise in the draw.io configuration.

See more examples of [smart templates and generated diagrams](/blog/smart-diagram-generation.html).
<br /><img src="/assets/img/blog/generate-mockup2.png" style="width=100%;max-width:500px;height:auto;" alt="The new generate diagram tool">