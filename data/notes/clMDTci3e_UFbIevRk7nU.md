
## Summary

This describes Dendron's weekly planning process. Think of it as sprint retrospectives, Dendron style.

## Process

### Before
- @weeklyPlanner 
  - create `weekly.journal.{date}`
  - create `weekly.journal.2021.11.16.plan` (this will create a note with the planning checklist [^lead])
- @everyone: copy the weekly planning user [^user] template and go through checklist ^QVIJ3imkWAEo

### During
- during the meeting, we recommend that those following along have two windows of the google doc open
  - one window to follow along the current section
  - another window to add any [[Next items|templates.weekly-planning.gdoc#next]] or [[Discussion|templates.weekly-planning.gdoc#discussion]] you want to bring up based on whats currently being discussed

### After
- @weeklyPlanner: go through [[After Meeting Checklist|templates.weekly-planning.lead#after-meeting]]
- @everyone: [[weekly Journal|handbook.sop.weekly-journal]]


### Update Next Week Milestones
1. Create a [new milestone](https://github.com/dendronhq/dendron/milestones/new)
  - version is one minor version above current version (eg. if we're currently on `v55`, next week would be `v56`)
  - due date is Tuesday of next week
1. Move tasks from [Up Next Milestone](https://github.com/dendronhq/dendron/milestone/16) into next weeks milestones
1. Assign owners to these tasks

### Update This Week Triage
1. For all issues from oncall that are on triage, add it to the [[Triage|templates.weekly-planning.gdoc#triage]] section of weekly planning

### Update CROP
- See [[Crop Community Issue|dendron://private/dendron.sop.crop-community-issue]]
1. Announce in the `#feedback` channel the CROP of this week. Tag the original submitter in the response if possible
1. Update [[Crop Tasks|dendron.tasks.crop]]
  - add voted on CROP to active
  - move other crops to the bottom of [[Previous|dendron.tasks.crop#previous]]
1. Make sure there 3 CROP items for [[Next|dendron.tasks.crop#next]]

##

[^lead]: [[templates.weekly-planning.lead]]
[^user]: [[templates.weekly-planning.user]]
[^team]: [[templates.weekly-planning.team]]
[^gdoc]: [[Gdoc|templates.weekly-planning.gdoc]]