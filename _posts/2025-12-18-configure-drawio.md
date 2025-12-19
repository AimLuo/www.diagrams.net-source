---
layout: post
author: draw.io
slug: configure-drawio
date: 2025-12-18 09:54:00
title: Customise and configure the draw.io editor to diagram faster
tags: [features]
categories: [features]
---

The draw.io editor has a mountain of configuration options that can make your diagramming faster. Set custom colour palettes, styles, fonts, shape libraries, templates, and even editor themes, enable or disable certain features, set defaults for connectors, and more via the extensive draw.io configuration options. 

As draw.io is available as an online editor, as apps in content platforms, as an [offline Desktop app](/blog/desktop-secure-diagrams.html), and embedded in [various integrations](/integrations.html), not all configuration options are available across all platforms and integrations. For example, [draw.io for Confluence has many additional features and options](/doc/drawio-confluence-cloud-admin.html) that can only be configured inside Atlassian's app administration settings, that are not available in the online editor. 

**Tip:** draw.io configuration options are written using a [JSON string](http://www.json.org/). To ensure the configuration is valid JSON use a [validator such as JSONLint](https://jsonlint.com/). and make sure you replace double-escaped quotes (\\") with single-escaped quotes (\").

**Open the draw.io configuration**

Select _Extras > Configuration_ from the draw.io menu (Classic, Atlas editor theme), or _Settings > Configuration_ from the draw.io menu(Simple, Minimal, Sketch themes).
<br /><img src="/assets/img/blog/extras-configuration-menu.png" style="width=100%;max-width:400px;height:auto;" alt="Access the draw.io configuration via Extras > Configuration">

## Configure default styles

Restyling shapes and connectors after you have added them to the diagram takes a lot of time. If you always use the same colours (such as when you must follow a corporate style), set them up in the draw.io configuration as custom presets or colours that are used by default.

Set up a **custom palette** (``presetColors``, ``customPresetColors``, ``defaultColors``) and colour schemes (``customColorSchemes``, ``defaultColorSchemes``) with default and preset colours to make colouring your diagram faster. 
<br /><img src="/assets/img/blog/preset-colours-new-defaults.png" style="width=100%;max-width:200px;height:auto;" alt="The default present colours can be customised in draw.io">

Specify how **adaptive colours** (``defaultAdaptiveColors``, ``enableLightDarkColors``) automatically switch when you use dark or light mode in your browser. 
<br /><img src="/assets/img/blog/style-colour-palette-custom.png" style="width=100%;max-width:500px;height:auto;" alt="An additional custom colour scheme has been added to the style palette in draw.io">

Set **custom and default fonts** and styles for text labels (``customFonts``, ``defaultFonts``) if your company has a style guide that requires you to use specific licensed or web fonts. 
<br /><img src="/assets/img/blog/custom-fonts-multiple-confluence-cloud.png" style="width=100%;max-width:400px;height:auto;" alt="Multiple custom fonts can be used in draw.io for Confluence Cloud">

You can also set **default styles**, lengths and label styles for connectors (``styles``, ``defaultVertexStyles``, ``defaultEdgeStyles``).

[See all the style configuration options available in draw.io](/doc/faq/configure-diagram-editor#format) - there are many more than are listed above.


## Add custom libraries and templates

You can make your own **custom shapes** in draw.io, draw freehand shapes, and edit connection points on existing shapes, and then these in custom libraries. 

In the draw.io configuration, you can set these custom libraries or any of the built-in draw.io shape libraries to load by default (``defaultLibraries``, ``enabledLibraries``, ``libraries``, ``defaultCustomLibraries``).
<br /><img src="/assets/img/blog/custom-templates-imported-library.png" style="width=100%;max-width:300px;height:auto;" alt="An imported custom library will appear in the shapes panel on the left in draw.io">

If you want to disable custom libraries completely, or set newly enabled libraries to appear already expanded, you can do that too. (``enableCustomLibraries``, ``expandLibraries``)

To setup a **custom template library** (``templateFile``), you need to create an [XML file containing a list of all custom (and default) templates and custom shape libraries](/doc/faq/format-template-library.html) that the templates open by default. This is used to list the template categories and their diagrams in the template library dialog. 
<br /><img src="/assets/img/blog/template-library-custom.png" style="width=100%;max-width:400px;height:auto;" alt="You can configure draw.io to use a custom template library with your own diagram templates and custom shape libraries">


## Customise draw.io editor features

There are many more features in draw.io that can be tweaked to help you reach the final diagram faster, including:
*  how the sidebars appear around the canvas
*  how the mouse is used to zoom in/out and paste shapes
*  custom grid sizes for the drawing canvas
*  custom page formats
*  ...  

To get past that blank page and started diagramming faster, the draw.io diagram generation features enable you to draw a diagram from a simple text description. These diagram generation settings are also configurable. 

**Diagram generation features** are enabled by default in the online draw.io editor and use a variety of online AI models. You can generate a diagram via _Arrange > Insert > Generate_ in the menu, in the [template manager](blog/smart-diagram-generation.html), in the [shape search field](/blog/search-omnibox.html) and via the [sparkle tool](/blog/generate-diagram-tool.html). 

* In draw.io for Confluence, these features are _disabled by default_. As an administrator, set ``"enableAi": true`` in the draw.io app configuration in your instance's administration settings to allow your users to generate diagrams.

* Diagram generation is not available in the offline draw.io Desktop app. 

Via the draw.io configuration, you can [customise which LLM models to use](/doc/faq/ai-customisation.html), the actions available via the [search omnibox](/blog/search-omnibox.html), the default instructional prompts for each action, and more.

For example, the Generate dialog below lets you select various [diagram generation actions and specific models](/doc/faq/configure-ai-options.html), all customised via the draw.io configuration. 
<br /><img src="/assets/img/blog/configuration-custom-ai-actions-endpoints.png" style="width=100%;max-width:400px;height:auto;" alt="The diagram Generate options can be customised in draw.io to include specific actions or allow you to choose specific AI models">

Take some to set up your configuration well and you can seriously optimise your diagramming workflow to start and finish your diagrams faster.






