---
id: euhmlM2v57OZoWIl9CQ67
title: Issue Management
desc: ''
updated: 1642373756706
created: 1639779529417
---

## Summary
How to track your tasks in Dendron

## Prerequisites
- [[Issues in Airtable|dendron://dendron.handbook/area.team.sop.issues-in-airtable]]

## Steps

### Create your own dashboard

See [[Create Your Own Task Dashboard|dendron://private/area.team.sop.issue-management.sop.create-your-own-task-dashboard]]

### Working with tasks

1. When creating a task, follow steps in [[Creating New Issues|dendron://dendron.handbook/area.team.sop.create-new-issue]]
1. After the task has been created, update it as necessary by exporting to airtable when the [[status|dendron://private/task.temp.ref#status]] changes
    - when `status = review`, add the [[pull request|dendron://private/task.temp.ref#pr]] url to the task
    - when code is checked into master, set `status` to `checked`
    - when the code is pushed to master, set `status` to #status.pushed
    - when the code is released, set `status` to #status.released

- NOTE: don't forget to export the task after updating the status

### Adding a task as a crop
- add #kind.crop to the note metadata
- NOTE: if the task is internal, add #type.chore to it

See more about [[CROP|dendron://dendron.dendron-site/community.events.crop]]

### Adding a task to the icebox
- add #kind.icebox to the note 

An icebox item is something we are not working on for +1 year (if ever)

### Adding a task to the team backlog
If you have items in your backlog that you don't think you have time for, you can add it to the team backlog by removing yourself from the `owner` field. 

This will move the task to the [[Team Backlog View|s.airtable.ref.base.tasks.tasks#^0h8oCnzIXtAB]].

- NOTE: if you're still interested in doing the task but don't have time to do it soon, set the [[due|dendron://private/task.temp.ref#due]] date to be 2 months from today and it will also show up in the backlog view to indicate that others are free to work on this 

### Cleaning up tasks after a sprint
- NOTE: the old sprint complets and the next sprint starts on [[Tuesdays 9PM UTC every week|dendron://private/dendron.ref.calendars#^EN8PYxT1NkFQ]]
1. If the task has been completed, delete the sprint key front the note
1. Go to airtable and delete the sprint key 
1. All tasks that are tagged #sprint.next should now be switched to #sprint.active

- TIP: cleaning up is a bit cumbersome right now due to some missing functionality with tasks and exports. you can make it easier by doing the following
    1. make sure you have a keyboard shortcut set for export task, see [[Export Keyboardshortcut|dendron://private/area.team.sop.issue-management.sop.export-keyboardshortcut]]
    1. in your weekly journal, add a section called `Tasks` and c/p all your tasks there (eg. [[Tasks|dendron://private/user.kevin.weekly.2022.01.11#tasks]])
    1. after the sprint is over, go in and update all your tasks release status
    1. go to the task pod config  and comment out `exportScope`: [[pods/custom/config.dendron.tasks.yml]]
    1. select all the tasks you updated and use the keyboard shortcut to trigger export task 
        - TODO: currently there is a bug where the export no longer shows up if you remove the scope
        - this will updated all selected tasks
    1. go to the sprint active [^sprint-active] view on airtable and delete the sprint tag
        - TODO: we currently don't support deleting a single select
    1. uncomment the `exportScope` comment 

## Examples

## Checklist
<!-- Optional, use to check if sop is accomplished -->

## Related
- All tasks views: [[here|s.airtable.ref.base.tasks.tasks#tasks]]

[^sprint-active]: [[Tasks|dendron://private/s.airtable.ref.base.tasks.tasks.views#^u56XOun5P9xg]]
