---
id: 4hdvg4q0hppl10hhadn06p9
title: Notes
desc: ''
updated: 1654624182416
created: 1654621971901
---
@everyone

Dendron 0.98 has sprouted  🌱
https://wiki.dendron.so/notes/14h6ul847l9o4ve0rlfshcs/

**Template Helpers:** Templates just got more powerful in Dendron. Make your notes programable using built-in helpers like equality checking or date fetching. 
- More information: [[Template Helpers|dendron://dendron.dendron-site/dendron.topic.templates.template-helpers]]

**Custom Themes in Preview**: You asked for it and now its here. Customize the preview with your own css (and share them in our new #themes channel).
- More information: [[Theme|dendron://dendron.dendron-site/dendron.topic.theme]]

**Hovers Are Coming to Backlinks**: Backlinks will now preview the contents of the note when hovering over a link.
- More information: [[Backlinks|dendron://dendron.dendron-site/dendron.topic.sidebar.backlinks]]

### Deprecated 
Old style templates are being replaced with [[Handlebar Templates|dendron://dendron.dendron-site/dendron.topic.templates.handlebars]]. See the [[migration guide|dendron://dendron.dendron-site/dendron.topic.templates.handlebars.migration]] for changes.

## Highlights
- feat(views): preview uses your vscode theme colors  
- feat(views): custom theme support for preview 
- feat(navigate): backlink panel with hover
- feat(edit): template helpers 

## Everything Else
- enhance(view): decrease min zoomed font-size for node labels in graph panel
- enhance(workspace): "migrate to self contained vault" updates `logopath` and moves gitignore file 
- enhance(extend): add axios to hook function 
- fix(publish): export gets stuck if `logoPath` is set but the logo doesn't exist
- fix(views): added default initial theme for webviews
- fix(views): bullet points missing in new theme-matching style
- fix(views): backlinks panel tweaks
- fix(views): images with encoded uri are not rendered in the preview
