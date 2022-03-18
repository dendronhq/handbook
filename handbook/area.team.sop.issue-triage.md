---
id: mXJCZEpIm5y8DnFS7qZUs
title: Triaging Issues
desc: ''
updated: 1639780595184
created: 1637971384061
---

## Summary
How we triage (categorize) new issues. 

An issue can be anything from github or something created by a team member as part of the weekly planning process.

## Steps
1. Triage the task:
    - if the item is **high priority**
        - add [[tags.sprint.active]] label to the task
        - attempt repro immediately and assign an engineer for immediate investigation
    - add the appropriate [[tags.scope.{scope}]] to the task
        - Valid values can be found in the `tags.scope.*` hierarchy
        - This should match the hierarch of the note (i.e. `task.lookup.blah`)
    - add an approximate size to the tags.size field, if possible
    - if the item is a good crop candidate
        - add [[tags.crop]] to the task
        - respond with the following [[template in the issue|dendron://private/dendron.sop.triage.temp.crop]]
    - Other fields are non-essential and can be left blank
1. Upload the task to Airtable with this sop: [[Issues in Airtable|dendron://dendron.handbook/area.team.sop.issues-in-airtable]]

## Examples
- [[Podsv2 Edit Config Command|dendron://private/task.pod.podsv2-edit-config-command]]

## Related
- [[Triage GitHub Issue|dendron://dendron.docs/dev.process.issues.sop.triage-github-issue]]

## Next Steps
- [ ] update the following documents:
    - [[Triage|dendron://private/dendron.sop.triage]]
    - [[Monthly Triage|dendron://private/dendron.sop.triage.monthly]]
