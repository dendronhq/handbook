---
id: t2lzhsuxqeki7fg7c1i5vl3
title: Notes
desc: ''
updated: 1657036577567
created: 1657035672840
---
@everyone

Dendron 0.102 has sprouted  🌱
https://wiki.dendron.so/notes/ijgipdvbffakeq7n0b6k9eq/

**New Visualization Command for Workspace**: Check out our new CLI command that shows large amounts of data with hierarchal relationships as packed-circles, and helps you navigate through them more efficiently!
- More Information: [[Packed Circles|dendron://dendron.dendron-site/dendron.topic.packed-circles]]  

## Highlights
- feat(cli): add a cli command that generates a packed-circles visualization of workspace 
- enhance(markdown): add new template variables

## Everything Else
- enhance(publish): add "link to anchor" icon by headings and block anchors
- enhance(publish): faster rendering of sidebar in published site 
- fix(workspace): sync fails in shared workspaces if users update workspace config first before syncing migrated vaults 
- fix(structure): quickpick stuck issue for refactor hierarchy cmd 
- fix(workspace): removing vault with a name different than their `fsPath` doesn't remove them from `duplicateNoteBehavior` 
- fix(workspace): duplicate note id detected even after a file is removed 
- fix(views): backlink tree item labels are trimmed excessively 
- fix(publish): regression where publishing fails if note doesn't exist 
- fix(workspace): fix init in workspace without workspace folders 