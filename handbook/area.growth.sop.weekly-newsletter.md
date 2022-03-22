---
id: aJvjn7cztfZ3ctRK
title: Weekly Newsletter
desc: ''
updated: 1647971908995
created: 1628011914293
---

## Summary

Dendron sends out a weekly newsletter, scheduled for every Wednesday at 6AM PST.

## Prerequisites

- [[PodV2 Quickstart|dendron://dendron.dendron-site/dendron.topic.pod-v2.quickstart]]
  - We need to have the Markdown Export Pod configured so that we can copy the contents of the release notes to the clipboard with all URLs properly converted.

## Steps

- Open a new scratch note
- Insert the weekly newsletter template: [[Newsletter|dendron://dendron.handbook/area.growth.sop.weekly-newsletter.temp.newsletter]]
  - Follow the TODO items in the template
- Run `Export Pod V2` and export the content of the scratch note to clipboard
- Login to [Buttondown](https://buttondown.email/)
  - Password should be available within the Dendron password vault. Reach out to the team if it isn't appearing, as you may need permissions.
- Once logged in, you should be at a page for writing a new email. Paste what is in your clipboard into the body of the email.
- If the release notes have indented bullet points (in the contributor section, events section, etc.), make sure each indent is **four spaces**. This is because Buttondown doesn't seem to acknowledge when there is only two spaces used for indentation in lists. Use the email preview to confirm the formatting will be working as expected.
- Confirm that the email includes no broken links (Buttondown will show a warning if it discovers any, and will show these below the email near the scheduling buttons).
- Schedule the email for Wednesday at 6AM PST.

## Template
- [[Newsletter|dendron://dendron.handbook/area.growth.sop.weekly-newsletter.temp.newsletter]]
