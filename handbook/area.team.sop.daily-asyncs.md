---
id: 5Jgi3mnbKHzTBNW4nVzJb
title: Daily Asyncs
desc: ''
updated: 1646323574761
created: 1640911424474
documentId: 1Nug8iNj716m3GsTTMy5M-bVi5wjCL1uCzEdgB-__hIU
published: false
revisionId: >-
  ALm37BXxPTIhkFjanUF-dvB830X29nYvWQWvGYoeQUMj5Cgd7EwSRg1bGzzkvO9DsuErSzRbCwMRcL0Fll2qQg
---

## Summary

Daily Asyncs are where all asyncs are posted. 
are our source of truth for all discussions and announcements that the entire team is involved in

## Context

Its easy to lose messages in discord, especially announcements. Daily asyncs

this gives us one source of truth for all team wide announcements

## Steps

### Creating
1. When you schedule an [[Async Meeting|dendron://dendron.handbook/handbook.sop.async-meetings]], add a link to it to `meet.daily` under the current date 
  - If no date exists for today, create one
  - If date exists, add your async to the top of the list
    - It is easy to look at the first item under the day and think there are no outstanding asyncs that need your acknowledgement. For this reason, adding a new async to the bottom makes it easy to be missed.
  - cutoff time for a given date is 23:59PM UTC of the same day
  - format: 
      ```
      - @{username}: {Proposal} - {document link}
      ```
  - example
      ```md
      - @kevin: Pod change proposals - https://docs.google.com/document/d/***/edit
      ```

### Responding
1. Dendron team members should [[add an acknowledgement|dendron://private/area.team.sop.weekly-planning-commenting#adding-an-acknowledgement]] for all previous day asyncs within 24h of the day

### Archiving
1. The daily meeting notes for a given day will be imported into the `meet.daily.{date}` hierarchy every week on Wednesday. 
    - NOTE: on Thursday, notes from previous Wednesday to this week Tuesday midnight will be imported and then erased from the google doc

## Reference
- [[Daily Async GDoc|dendron://private/s.gdocs.ref.daily-async]]