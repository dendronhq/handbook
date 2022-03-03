---
id: 9bacfb70-5777-4fc4-b069-f902f42762b9
title: Async Meetings
desc: ''
updated: 1646002125054
created: 1622383410206
---


## Summary

At Dendron, we try to be async first. Async meetings let us collaborate across different timezones. This involves setting a date, inviting relevant parties, and having a shared gdoc that participants can comment on.

The purpose of these should be to encourage discussion, brainstorming, or decision making.

Examples of good use cases - going over a design doc, discussing product strategy, etc.

## Steps

### Mini Async

Use this when you made a small update to the handbook/site/etc and want to do a lightweight async. See [example](https://github.com/dendronhq/handbook/commit/58aa4d75c1d5275c01e628dd77e24a99a216748f#)

1. Create a new thread in the `#async-meet` channel and set expiration for 24h (this should be the default)
  - NOTE: if you are creating on Friday, set expiration to 3D
  - the title of the channel should be `mini: {TITLE}`
1. Link to the commit/scratch note in question and mention the `@DendronTeam`
1. Team members have 1 business day to respond to the thread, either with comments or a 👍 to acknowledge reading

### Planner
1. Open the team google drive [^async]
  - click the **+ New** button on the top left, select google doc, and select **Create and Share**
  - use the [[meeting template|dendron://dendron.handbook/templates.meet]] as the general outline for the meeting
1. create a calendar invite with the following:
  - Title: [async] "What you need done"
  - Guests: anyone who needs to get things done with you (but working separately)
  - Location: At your desk.
1. create a discord post in `#async-meet` sharing the details of the event. Use the discord template [^discord]
1. 24h after the meeting, copy the meeting notes back into the workspace under `meet.journal.{date}.{topic}`
1. ping relevant parties when the meeting is done

### Attedant
1. If you attended the meeting, please leave a 👍 in the original announcement to notify that you have reviewed the doc

## Templates
- [[Meet|dendron://dendron.handbook/templates.meet]]

## Reference

### Team async meetings

These are tracked (like other company-wide meetings) in our [shared calendar](https://calendar.google.com/calendar/embed?src=c_hdk7vjft9ch2meqqk6mfq5a2v8%40group.calendar.google.com&ctz=Asia%2FKolkata).

- Weekly planning
  - pre-meeting project update.
  - post-meeting update of user.\*.weekly notes.

### Individual async meetings
Recommended and optional async meetings for yourself. Any subset of the following may work for you:
- [Daily] Journal update
- [Daily] Morning planning
- [Daily] Evening review/next day journal creation.
- [Weekly] Review tasks assigned to you in Github so they're up to date.


[^discord]: [[Discord|dendron://dendron.handbook/handbook.sop.async-meetings.temp.discord]]
[^async]: [[Google|dendron://private/dendron.ref.google#^xAiAodi9KuR4]]