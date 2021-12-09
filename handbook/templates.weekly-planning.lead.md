---
id: xgIjSQJcQyGArCDKKH9an
title: Weekly Planning Lead Checklist
desc: ''
updated: 1638889174303
created: 1625575868274
---

## Checklist

### Before Meeting
- Before Monday
  - [ ] Create next weekly journal using `weekly.journal.{date}` 
  - [ ] Close previous week's milestones in Github
  - [ ] [[Update Next Week Milestones|handbook.sop.weekly-planning#update-next-week-milestones]]
  - [ ] Announce results of last week triage
  - [ ] Finish [[individual weekly planning|templates.weekly-planning.user]]
  - [ ] Announcement weekly planning (create a new thread in `#dendron-team` titled `weekly-planning {date}`) using the following [[template|templates.weekly-planning.team]]
      - NOTE: date should be the for the following tuesday (eg. on 2021-10-31, date should be 2021-11-09)
      - NOTE: thread should be set as 3 days to auto archive
  - [ ] look at `tags.sprint.next` <!-- [[tags.sprint.next]] --> and assign
  - [ ] [[Update CROP|handbook.sop.weekly-planning#update-crop]] (every other week)

- By Monday
  - [ ] Assign this week's [[dendron.sop.crop-community-issue]]
  - [ ] Remind stragglers to update the gdoc (EOD Monday)


### After Release
  <!-- We'll automate this process, right now, not worth doing-->
- [ ] Ensure current [milestone](https://github.com/dendronhq/dendron/milestones) tasks are in the weekly journal.
  - Tasks should be obtained from people's current goals
- [ ] Update [[rfc]] so it's current.
- [ ] Close out last week's weekly journal [^1]
- [ ] Remind people to update issue in Github [^2] 
- [ ] Go over previous and current goals
- [ ] Upload video via [[Weekly Planning Recording|dendron://private/area.team.sop.weekly-planning-recording]]

### One Day After Meeting
- [ ] Move notes from gdoc to `meet.planning.{year}.{MM}.{{dd}`
- [ ] Set up next week's gdoc [^meet-gdoc] with a clean template to allow people time to fill it out.
- [ ] go through issues in [[Triage|templates.weekly-planning.gdoc#triage]] where items will end in one of the following places:
    - [[backlog issue|dendron.tasks.backlog]]
    - [[crop issue|dendron://private/dendron.tasks.crop#next]]
    - assign it to a team member for this current sprint
    - assign it as an upcoming [[project|dendron://private/proj#next]]


##

[^1]: [[Weekly Journal|weekly.temp.team-journal]] 
[^2]: [[After|templates.weekly-planning.team#after]]
[^meet-gdoc]: [meet gdoc](https://docs.google.com/document/d/1GEZfMMHLmz5AIvGoZrjM24TL7r_XjlmuerjEa2L9Pmo/edit#)
