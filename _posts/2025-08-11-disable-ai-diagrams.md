---
layout: post
author: draw.io
slug: disable-ai-diagrams
date: 2025-08-11 09:24:00
title: Configure draw.io online to disable AI diagrams 
tags: [features]
categories: [features]
---

Like many software apps, diagramming tools now have AI-powered features that 'help' you diagram. These can be premium features and may not be easily disabled. With the free online draw.io editor, you have access to the diagram generation features by default. It's easy to disable this in draw.io - configure the editor or use the fully offline draw.io Desktop app. 

<img src="/assets/img/blog/configure-drawio-example.png" style="width=100%;max-width:400px;height:auto;" alt="All version of draw.io are highly configurable, with options for custom colours and fonts, and to enable or disable specific features">

**Note:** [Diagram generation features](/blog/smart-diagram-generation.html) are disabled by default in the draw.io apps for Confluence - ask your instance administrator to [configure the draw.io editor](/doc/faq/configure-diagram-editor.html) if you want to (and are allowed to) use this feature. 

While draw.io only shares the [text you enter as the query](/blog/write-query-generate-diagram.html) to generate a diagram, and only at the time of generation. 

draw.io does not share your diagram data with these LLM tools unless you specifically request that the generator modify your diagram or a selection of your diagram (this behaviour can be [customised or disabled in the draw.io configuration](/doc/faq/configure-ai-options.html)).

Note, other diagramming applications typically share your diagram data in full and by default with these generation tools, and do not allow you to customise or limit this behaviour. 

If you need to include sensitive data or draw confidential diagrams, your diagramming application must not share your diagram data.

## Use an offline tool like draw.io Desktop

Since version 10.7.5, draw.io Desktop has been a fully offline application. You do not need a connection to the internet to use all the built-in shape libraries and templates, or use your own custom shape libraries, fonts or templates stored on your device.

Diagram generation features are not available in [draw.io Desktop](/blog/diagrams-offline.html). 

<img src="/assets/img/blog/desktop.png" style="width=100%;max-width:500px;height:auto;" alt="The draw.io desktop app works on MacOS, Windows and Linux">

Choose your platform (Windows, macOS or Linux), and [download draw.io Desktop](https://get.diagrams.net/) to start diagramming securely and privately.

**Tip:** Many extra template and example diagrams are available in the [JGraph/drawio-diagrams](https://github.com/jgraph/drawio-diagrams) repository on GitHub. Download these in advance to use them in draw.io Desktop.


## Configure the draw.io web application

Alternatively, you can run the web app while offline as a [progressive web app](/doc/faq/offline.html), or configure the editor in your browser to disable the diagram generation features.

All versions of the draw.io application are highly configurable, including but not limited to:
* default palette colours and styles
* default and custom fonts
* custom templates and a customised template library
* default and custom shape libraries to automatically open by default 
* default page and grid size 

Here's a full list of the [draw.io editor configuration options](/doc/faq/configure-diagram-editor.html) for the web application, draw.io Desktop, and the draw.io apps for Confluence Cloud and DC.

Only the online draw.io web application has the diagram generation enabled by default. To [disable the diagram generation features](/doc/faq/smart-templates-disable.html), add a line to the editor configuration and refresh the tab to reload the draw.io editor. 

### Disable diagram generation in the draw.io configuration

This removes the Generate tool from template library and menu, the _Generate_ option from the [search field](/blog/search-omnibox.html), and the [sparkle tool](/blog/generate-diagram-tool.html) from the toolbar. 

**Note:** Be careful about capitalisation - draw.io configuration options are written using lower camel case (Java).

1. Select _Extras > Configuration_ from the menu, or _... > Settings > Configuration_ from the toolbar. 
<br /><img src="/assets/img/blog/extras-configuration-menu.png" style="width=100%;max-width:400px;height:auto;" alt="Access the draw.io configuration via Extras > Configuration">
1. Add the following JSON string to the configuration: ``"enableAi": false``
<br /><img src="/assets/img/blog/configuration-enableai-false.png" style="width=100%;max-width:300px;height:auto;" alt="Set the enableAI option to false in the draw.io configuration to disable the Generate in the template library, the Generate menu and search options, and the sparkle tool">
1. Click _Apply_ to save your changes. Reload the browser tab to load the new draw.io configuration and disable the diagram generation features. 

**Note:** If you set the [``lockdown`` option](/blog/data-governance-lockdown.html) to ``true`` in the draw.io configuration, this will also disable the diagram generation features. 

