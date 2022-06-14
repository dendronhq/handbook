---
id: k6c99vonug5q8yr296yrlb3
title: Notes
desc: ''
updated: 1655220348422
created: 1655220348422
---
@everyone
Dendron 0.99 has sprouted  🌱
https://wiki.dendron.so/notes/cpoqm8ed1q729m7lav31hhe/

**Better Task Notes**: Get things done - task notes now have custom commands to set their status and mark them as complete.
More information: [[Set Task Status|dendron://dendron.dendron-site/dendron.ref.commands#set-task-status]]

**Obsidian Import**: Vault to vault - we now have a dedicated command to import your notes from obsidian into Dendron!
More information: [[Import Obsidian Vault|dendron://dendron.dendron-site/dendron.ref.commands#import-obsidian-vault]]

## Highlights
- feat(structure): add set task status command
- feat(structure): add complete task command
- feat(sync): obsidian import flow

## Everything Else
- enhance(publish): make the private link colors customizable
- enhance(views): configure creation of notes on click of graph node with `createStubs`
- enhance(workspace): detect duplicate note id on lifecycle events
- fix(workspace): fix duplicated panel titles
- fix(edit): email addresses and hash symbols inside words are parsed as tags
- fix(views): gracefully handle tree view sort error to avoid crashing the tree view
