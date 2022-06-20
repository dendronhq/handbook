---
id: clMDTci3e_UFbIevRk7nU
title: Weekly Planning
desc: ''
updated: 1655724745228
created: 1624019624458
---

## Summary

This describes Dendron's weekly planning process. Think of it as sprint retrospectives, Dendron style.

## Steps

### Before
- [[Weekly Planner|dendron://dendron.handbook/role.weekly-planner]]
  - create `weekly.journal.{date}`
  - create `weekly.journal.2021.11.16.plan` (this will create a note with the planning checklist [^lead])
- [[Everyone|dendron://dendron.handbook/role.everyone]]
  - create `user.{username}.weekly.{date}.plan`
    - this will create a note with the [[Weekly Planning User Checklist|dendron://dendron.handbook/templates.weekly-planning.user]] ^QVIJ3imkWAEo
    - fill out the checklist prior to the meeting
#### Weekly Goals
1. Create a task note for each weekly goal ^ln5zq9jphkjb
      - NOTE: Even if there is an existing task note, create a new one specific to the weekly goal relating to the task
1. Every task note associated with a goal should be tagged with #kind.goal
1. Add a due date for sometime before the next weekly planning (Tuesday of next week)
1. Ensure the PR link is updated in the fm (where applicable)
1. Export task to airtable
1. Ensure it is visible on [[Weekly Planning Goals|dendron://private/ext.airtable.interface.weekly-planning-goals]]

### During
- during the meeting, we recommend that those following along have two windows of the google doc open
  - one window to follow along the current section
  - another window to add any [[Next items|templates.weekly-planning.gdoc#next]] or [[Discussion|templates.weekly-planning.gdoc#discussion]] you want to bring up based on whats currently being discussed

### After
- [[Weekly Planner|dendron://dendron.handbook/role.weekly-planner]]
  - go through [[After Meeting Checklist|templates.weekly-planning.lead#after-meeting]]
- [[Everyone|dendron://dendron.handbook/role.everyone]]
  - make any necessary updates in your [[weekly Journal|handbook.sop.weekly-journal]]

### Example
1. [[#weekly-goals]]

- [[user.bindhu.weekly.2022.06.21]]
```goal
## Current Goals
- [ ] [[Add Process for All Weekly Goals to Be a Task|dendron://private/task.2022.06.15.add-process-for-all-weekly-goals-to-be-a-task]]
```
- [[Add Process for All Weekly Goals to Be a Task|dendron://private/task.2022.06.15.add-process-for-all-weekly-goals-to-be-a-task]]
```fm
tags:
  - kind.goal
due: 2022.06.16
```

##

[^lead]: [[templates.weekly-planning.lead]]
[^user]: [[templates.weekly-planning.user]]
[^team]: [[templates.weekly-planning.team]]
[^gdoc]: [[Gdoc|templates.weekly-planning.gdoc]]
