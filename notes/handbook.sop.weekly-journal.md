---
id: CNP6_cMc1K8EtOEFi-e0P
title: Weekly Journal
desc: ''
updated: 1655376068883
created: 1623631213317
---

## Summary
The weekly journal is how we track tasks and priorities for individuals. It is also a good place to store tasks that are currently blocked or in the future.

Weekly journals are recorded in `user.{name}.weekly.*`

## Steps
1. Every monday, create a new weekly journal entry `user.{name}.weekly.{date}`
    - for Dendron, we start the week on Tuesday so have your `date` be the tuesday of the following week
    - eg. for user `bob` starting the process on `2021-09-06`, the next week entry would be `user.bob.journal.2021.09.14`, 
1. This will apply the [[Weekly Journal Template|dendron://dendron.handbook/templates.weekly-journal]] to your note
### For Weekly Goals
1. Before weekly planning:
    1. Create a task note for each weekly goal ^ln5zq9jphkjb
    1. Every task note associated with a goal should be tagged with #kind.goal and #sprint.next
    1. Add a due date for sometime before the next weekly planning (Tuesday of next week)
1. After weekly planning:
    1. For previous/completed goals, remove the #sprint.active tag and mark as complete
    1. For current goals, change from #sprint.next to #sprint.active