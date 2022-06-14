---
id: lctc12r51ur1bfby1ebihvy
title: Friction Log
desc: ''
updated: 1655154064054
created: 1655153549524
---

## Summary

Best practices for managing a [[Friction Log|dendron://dendron.handbook/area.team.concepts.friction-log]]

## Tips
- keep everything as a single note
- name it something easy to lookup (eg. `friction`)
- use the [[Entry|dendron://dendron.handbook/area.team.sop.friction-log#entry]] template to keep track of issues
- if applicable, email @kevin a copy of the friction log at the beginning of each day
    - NOTE: this doesn't apply if your a team member since everything is already in the team workspace
- [[Get Dendron Tracking UUID|dendron://dendron.handbook/area.common.sop.find-uuid]] and add it to the top of your friction log in the frontmatter

## Examples

```md
---
uuid: 076ea797-4fff-4d77-a169-a8e05c429848
---
### 2022-06-13
- had trouble refactoring hierarchy using `Refactor Hierarchy Command`
    - tried: running refactor hierarchy
    - resolved: google for "how regex works" 
```

## Templates

### Entry 
```
- {friction}
    - tried:
    - resolved:
```
