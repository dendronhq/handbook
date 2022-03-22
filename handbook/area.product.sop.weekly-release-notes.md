---
id: qsDq5jZVM0NqEmj7L2VgR
title: Weekly Release Notes
desc: ''
updated: 1647975014458
created: 1635724125776
---

## Summary
<!-- What is this SOP about -->
How to do release notes

## Steps

### Before the release
1. this will be a PR, so make sure your local `dev` branch is updated before creating a new branch related to the release
  - Recommended new branch naming scheme: `release-<version>` (ex. `release-083`)
1. update the changelog, see [[Changelog Update|dendron://dendron.handbook/area.product.sop.changelog-update]]
1. create a new release under `changelog.release.{date-with-dashes}`
    - NOTE: date should line up with the tuesday of the coming week and should be created in `dendron-site`
        - a template will fill after you create the note
    - eg. [[0.84|dendron://dendron.dendron-site/changelog.release.2022-03-01]]
    1. Fill out the highlights using [[Release Highlights|dendron://dendron.handbook/area.product.sop.release-highlights]]
1. Fill our community highlights using [[Community Highlights|dendron://private/dendron.sop.release.community-highlights]]
1. Add to and update everything under `## Community`
      - Starbord and TIL Highlights
      - Dendron Reading Series
      - [Event Reminders](https://lu.ma/dendron)
        - Make sure to include PST and UTC times
        - If Greenhouse Talk information is known, make sure the **Subject** and **Description** is populated.
      - Update Changelog range at bottom of release note
      - NOTE: the current oncall should have done the contributor updates for support issues in dendron repo, you should check `dendron-site` [^site] and `dendron-blog` [^blog] for additional issues
1. commit and push changes as an open PR
1. The evening before, create a new Discord thread in `#dendron-team` with the title `weekly-release yyyy-mm-dd`
  - Template: [[Discord Thread Start|dendron://dendron.handbook/area.product.sop.weekly-release-notes.temp.discord-thread-start]]
    - Make sure to change the values of hours estimate, and of the weekly journal names
        - Hours estimate: Amount of hours before 10AM PST
  - This is done to give the teams a heads up to get docs in, remaining updates to the `Ready to Ship` section, etc. ahead of time
  - Add second comment in Discord thread with link to release PR, tagging Kevin
    - ex. `@kevin In-progress release/changelog PR: <PR Link>`

### Day of release

1. ping @john about transferring community highlights to the release notes
    - He needs to create the `weekly.journal.*.contributions` contributor highlights
    - after john has finished transferring highlights, pull down changes and create a thread in `dendron-team` titled `weekly-release {date-with-dashes}` and use the [[Release|dendron://private/area.product.sop.weekly-release-notes#release]] template
1. after approval, merge changes to `master` and push
    - First confirm that `dev` currently includes all commits in `master`
      ```bash
      # In the dendron.dendron-site repo
      git checkout dev
      git pull # Gets latest changes
      git checkout master
      git pull # Gets latest changes
      git merge dev # Adds changes in dev to master
      git push # Publishes updated master
      ```
1. verify that changes are up
1. create release notes under `area.product.release.{date}.notes`
    - to create release notes, copy everything up to `# Community`
    - NOTE: make sure all discord mentions come out properly so that folks are notified for their contribution
    - example: [[Notes|dendron://private/area.product.release.2022.01.25.notes]]
1. create announcement notes under `area.product.release.{date}.announcement`
    - to create announcement notes copy everything in `# Community` but leave out `starboard` and `changelog`
    - NOTE: make sure all discord mentions come out properly so that folks are notified for their contribution
    - example: [[Announcement|dendron://private/area.product.release.2022.01.25.announcement]]


### After the release
1. Announce release on discord
1. Announce release on twitter
1. Announce release on mastodon

## Checklist
![[dendron://dendron.handbook/area.product.sop.weekly-release-notes.checklist]]

## Templates
<!-- Any additional templates (eg. release notes) that might be used -->

### Release 
Weekly release notes are ready in dev. Add an 👍 if all looks good

[^site]: [[Repos|dendron://private/s.github.ref.repos#^T8kaEVtPEEBC]]
[^blog]: [[Repos|dendron://private/s.github.ref.repos#^02M2XTWZQhKm]]
