# Obsidian templates

* [Templates - Obsidian Help](https://help.obsidian.md/Plugins/Templates) - Obsidian's native templating language

Obsidian has its own native templating language, which is what is used by the templates in the `Templates/` directory.

You can use things like `{{date}}` to insert a date string like 2023-07-01.

To insert these Obsidian templates, use the "Templates: Insert template" option from the command palette.

> [!Note] Templater plugin disambiguation
> The Templater plugin ignores Obsidian template tags and passes them through as is. The templates in the various other self-contained directories that use tags like `<% date.format('W, MMMM YYYY') %>` are using the Templater plugin. See [Introduction - Templater](https://silentvoid13.github.io/Templater/).
> These templates are used automatically when creating new notes within those directories from links that were inserted into the **Logbook** with like "Logbook template - new weekly review link", or by navigating the Calendar in the right sidebar
