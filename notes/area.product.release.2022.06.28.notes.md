---
id: aluvy8hnd8ekaqe3ricyvnc
title: Notes
desc: ''
updated: 1656432210351
created: 1656431859498
---
@everyone
Dendron 0.101 has sprouted  🌱

Last week, we launched on [product hunt](https://www.producthunt.com/posts/dendron-v100) and asked folks leave feedback. Thanks to the community, Dendron ended as the 5th most upvoted product of the day. Thank you everyone for your support 🙇‍♂️

**Depth Filter for Local Graphs:** Want to see the bigger picture? The graph depth filter now lets you control how much context you see in the [[Local Graph View|dendron://dendron.dendron-site/dendron.topic.sidebar.local-graph-view]]
- More Information: 
    - [[Other Filters|dendron://dendron.dendron-site/dendron.topic.graph-view#other-filters]]
    - [[Graph Depth|dendron://dendron.dendron-site/dendron._ref.web-ui#graph-depth]]

**Improved Note Traits:** Rust isn't the only language with traits! We've made a bunch of improvements to traits, including hot reloading, the ability to apply a template, bundling libraries like lodash and luxon, as well as better docs and error handling. 
- More Information: [[Traits|dendron://dendron.dendron-site/dendron.topic.traits]]

## Highlights
- feat(views): view more note links in local graph panel with depth customization 
- enhance(structure): improved note traits 

## Everything Else
- enhance(workspace): `Vault Add` command warns for unsupported transitive dependencies
- enhance(workspace): vaults always use UNIX style separators in config files 
- enhance(workspace): validate dendronrc.yml and emit error if invalid 
- enhance(edit): add match helper for hb templates 
- enhance(workspace): improve phrasing of sync message
- enhance(workspace): support single-vault workspace vaults for self contained vault migration 
- enhance(edit): reduce lag on autocomplete by adding a debounce 
- enhance(sync): adding import hint to tutorial
- fix(workspace): try to patch `EPERM` issues for windows
- fix(workspace): adding an existing remote vault avoids creating workspace files 
- fix(publish): issue publishing note with ref without a code-worksapce file
- fix(cli): dendron publish --help to display full list of arguments 
- fix(workspace): error when native workspaces are initializing 
- fix(publish): compile error with no banner present
- fix(structure): hot reload in note traits + no template by default
