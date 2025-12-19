---
layout: post
author: draw.io
slug: smart-diagram-generation
date: 2023-03-20 09:24:00
title: Smart diagram generation for more template diagrams
tags: [features]
categories: [features, import, templates]
---

When you create a new diagram with the [draw.io web editor](https://app.diagrams.net), you can now choose to use our new smart diagram generator instead of one of our existing templates. Describe your diagram in a text phrase, and the tool will generate a diagram based on what it parses. 
<br /><img src="/assets/img/blog/diagram-generator-template-library.png" style="width=100%;max-width:500px;height:auto;" alt="Generate diagrams of many different types from a text description via the template library in draw.io">

As these generated diagrams have not been vetted by a human, there are no guarantees it will useful as a template for your particular diagram. But the generated diagram can serve as inspiration, or a starting point from which you can draw the diagram you actually need.

**Tip:** You can generate endless variations of a diagram from the same phrase.

## Generate a template diagram in draw.io

1. Create a new diagram - go to [our online diagram editor](https://app.diagrams.net) - or click on ``+`` in the toolbar and select _Template_ to insert a generated diagram.
2. Click on the _Generate_ box in the template library.
<br /><img src="/assets/img/blog/diagram-generate-template-library.png" style="width=100%;max-width:300px;height:auto;" alt="Generate diagrams of many different types from a text description via the template library in draw.io"> 
1. Enter a basic description of your diagram in the text field, and press ``Enter`` or click _OK_.
<br /><img src="/assets/img/blog/diagram-generate-template-prompt.png" style="width=100%;max-width:300px;height:auto;" alt="Generate diagrams of many different types from a text description via the template library in draw.io">
2. Click _Insert_ or _Create_ to add it to the drawing canvas. 


<img src="/assets/img/blog/diagram-generator-template-library.gif" style="width=100%;max-width:500px;height:auto;" alt="Generate diagrams of many different types from a text description via the template library in draw.io">

Make sure you **write what type of diagram you want to generate at the start of the prompt**. In this example, the prompt was: 
<br />``sequence diagram - a customer purchases a product from a web store``


You can also generate a diagram via the menu and the toolbar:

* Use the shape search field above the Scratchpad - type in your prompt and select _Generate_. 
<br /><img src="/assets/img/blog/diagram-generate-search.png" style="width=100%;max-width:300px;height:auto;" alt="Generate diagrams of many different types from a text description via the search field in draw.io">

* Open the generate dialog via _Arrange > Insert > Generate_ in the menu, or click on the [sparkle tool](generate-diagram-tool.html), and then type in your prompt there. 
<br /><img src="/assets/img/blog/diagram-generate-tool.png" style="width=100%;max-width:300px;height:auto;" alt="Generate diagrams of many different types from a text description via the menu and toolbar in draw.io">

**Tip:** Hover over the generated diagram or click on the magnifying glass in the top right of the template preview or below the generated diagram to see a larger version before adding it to the drawing canvas. 

You can now edit, add to, delete, and style the shapes and connectors in the generated diagram.

<br />
## Different types of generated diagrams

Here are some different types of diagrams generated from the phrase "a customer purchases a product from a web store".

<img src="/assets/img/blog/diagram-generator-flow.png" style="width=100%;max-width:250px;height:auto;" alt="Generate a flowchart from a text description via the diagram generate dialog in draw.io"> 
<img src="/assets/img/blog/diagram-generator-sequence.png" style="width=100%;max-width:350px;height:auto;" alt="Generate a UML sequence diagram from a text description via the diagram generate dialog in draw.io"> 
<br /><img src="/assets/img/blog/diagram-generator-state.png" style="width=100%;max-width:200px;height:auto;" alt="Generate a state diagram from a text description via the diagram generate dialog in draw.io">
<img src="/assets/img/blog/diagram-generator-er.png" style="width=100%;max-width:350px;height:auto;" alt="Generate an entity relationship model from a text description via the diagram generate dialog in draw.io">

Of course, that phrase won't generate something useful for certain types of diagrams, like this Gantt chart. 
<br /><img src="/assets/img/blog/diagram-generator-gantt.png" style="width=100%;max-width:400px;height:auto;" alt="Generate a Gantt chart from a text description via the diagram generate dialog in draw.io">

And because the previous phrase makes no sense when describing a mindmap, here's "types of technical diagrams for IT workers".
<br /><img src="/assets/img/blog/diagram-generator-mindmap.png" style="width=100%;max-width:400px;height:auto;" alt="Generate a mindmap from a text description via the diagram generate dialog in draw.io">

[_Open all of these generated examples in a multi-page diagram in our diagram viewer_](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&page=0&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fsmart-generated-diagrams-examples.drawio)

### More ways to generate diagrams from text

In draw.io, there are many different ways to generate diagrams automatically from text.
  
* [Mermaid](/blog/mermaid-diagrams.html) - all UML diagram types, as well as pie charts, flowcharts, organisation charts, Gantt charts, Sankey diagrams, pie charts and more. 
  
* [Entity diagrams](/blog/insert-sql.html) - from SQL code.
  
* [CSV data into diagrams](/blog/insert-from-csv.html) - with formatting information to create flowcharts, mindmaps, org charts, directed graphs and more.


## Troubleshooting generated diagrams

Some diagram types lend themselves more naturally to text descriptions. Flow charts, sequence diagrams and mind maps are easier to generate than git graphs from a text description. 

As this tool is not a human and can not know what is logical to include in a diagram, there are no guarantees you will generate a diagram that is fit for purpose.

This feature uses a third party service to parse your phrase, and it can get somewhat overloaded at times. 

* Click _Refresh_ if the Generation dialog process times out.
  
* If the keywords in your phrase cannot be adequately parsed to generate a diagram, you may receive an "Diagram not found" error or a basic flowchart template. Try another descriptive phrase and regenerate your diagram.

## Generated diagrams in draw.io for Confluence and Jira

[Diagram generation features are disabled by default](/doc/faq/confluence-cloud-enable-smart-templates.html) if you are using the draw.io app for Confluence Cloud. Ask your administrator to enable this option in the draw.io configuration.