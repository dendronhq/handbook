---
id: qcX1EYCDe3Z2S8xDFfOkT
title: Ready to Ship
desc: ''
updated: 1656472203633
created: 1636474044281
---

## Summary

How to add an entry to [[Ready to Ship|dendron://private/weekly.temp.team-journal#ready-to-ship]].

- NOTE: this is relevant for anyone that merges changes into master

## Steps
1. After a PR has been merged, add it to the correct triage area in the weekly [^ship]
![[dendron://dendron.handbook/area.product.sop.ready-to-ship.notice-release-schedule]]
1. Ensure that the correct type [^type] and scope [^scope] are assigned
1. If the PR has multiple features, add in each feature separately. Feature breakdown should be included in the PR details when [[Submitting|dendron://dendron.docs/dev.process.review#submitting]] it. 
1. Ensure the format for [[Pull Request title|dendron://dendron.docs/dev.process.review#pull-request-title]] is followed
1. Add the alias of the user
1. If the change affects user behavior, add `([[docs|{link-to-docs}]])` at the end of the message
1. Sync your workspace (it is likely that multiple people are editing this doc)

## Examples

### Commit with no docs

- NOTE: no docs needed since this doesn't introduce new behavior

```md
enhance(publish): make publishing faster @john 
```

### Commit with docs

```md
enhance(publish): introduce cat footer as a configurable footer @john ([[docs|dendron.topic.publish#fancy-cat-icon]])
```

### A entire release
- [[Ready to Ship|dendron://private/weekly.journal.2021.11.09#ready-to-ship]]

## Checklist
<!-- Should be used to do the task -->

## Templates
<!-- Any additional templates (eg. release notes) that might be used -->

[^ship]: [[Ready to Ship|dendron://private/weekly.temp.team-journal#ready-to-ship]]
[^scope]: [[Assign Scope to Feature|dendron://dendron.docs/dev.process.review.sop.assign-scope-to-feature]]
[^type]: [[Assign Category to Task|dendron://dendron.docs/dev.process.review.sop.assign-category-to-task]]
