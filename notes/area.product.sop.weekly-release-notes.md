---
id: qsDq5jZVM0NqEmj7L2VgR
title: Weekly Release Notes
desc: 'How to do release notes.'
updated: 1654270001976
created: 1635724125776
---

## Summary

{{fm.desc}}

## Details

Release notes are done with the General Release of Dendron that comes out each Tuesday. These provide quite a bit more context compared to the changelog notes, including:

- Highlights
- Upcoming events
- Discord community messages from the [[today-i-learned|dendron://dendron.dendron-site/community.discord.channels#today-i-learned]] and [[starboard|dendron://dendron.dendron-site/community.discord.channels#starboard]] channels
- Community contributions: Contributors that have been raising issues, contributing code, contributing docs, etc. For more information, view the documentation on [[Discord Roles|dendron://dendron.dendron-site/community.discord.roles]]
- General announcements: Blog posts, videos, other events/resources of note, etc.

The release notes also serve as the content submitted to subscribers of the Dendron Newsletter.

## Steps

### Before the release
- due: 23:00 UTC Monday

1. Run `workspace sync` in your local `dev` branch for `dendron-site` vault
1. Create a new release branch with format `release/<version>` (eg. `release/083`)
1. Update the changelog > [[Changelog Update|dendron://dendron.handbook/area.product.sop.changelog-update]]
1. Create a new release under `changelog.release.{date-with-dashes}`
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
- Video example: https://youtu.be/UTEHbTO5bnA?t=1597

1. ping @john about transferring community highlights to the release notes
    - He needs to create the `weekly.journal.*.contributions` contributor highlights
    - after john has finished transferring highlights, pull down changes and create a thread in `dendron-team` titled `weekly-release {date-with-dashes}` and use the [[Release|dendron://private/area.product.sop.weekly-release-notes#release]] template
1. after approval, merge changes to `master` and push
    - First confirm that `dev` currently includes all commits in `master`
    - Once confirmed, merge `dev` into `master`
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
1. use markdown export pod to copy to clipboard on release notes (ensure wikilinkToUrl is true)

1. create release notes under `area.product.release.{date}.notes`
    - NOTE: loom video embed links will not render in discord, use a regular loom link instead (eg. https://www.loom.com/share/c6e8e75605d5416a9a8aa67465a6df17)
    - Add `@everyone` to the top
    - to create release notes, copy everything above `## Community`
    - This should include:
      - Release Highlights descriptions
      - **Highlights** section
      - **Everything Else** section
    - example: [[Notes|dendron://private/area.product.release.2022.01.25.notes]]
    - Add the URL link to the release directly beneath `Dendron {version} has sprouted`
      - example:
        ```markdown
        Dendron 0.87 has sprouted  :seedling:
        https://wiki.dendron.so/notes/qcwfzax4uaqj54evgp8li5y/
        ```
1. create announcement notes under `area.product.release.{date}.announcement`
    - Add `@ServerNotify` to the top
    - to create announcement notes copy everything in `## Community` but leave out **Starboard**, **Changelog**, and **Reading Series** sections
    - This sections should include:
      - **General**
      - **Events**
      - **Thank Yous**
    - NOTE: make sure all discord mentions come out properly so that folks are notified for their contribution
    - example: [[Announcement|dendron://private/area.product.release.2022.01.25.announcement]]
1. create reading series notes under `area.product.release.{date}.reading-series`
    - Use [[Template|dendron://dendron.handbook/area.product.sop.reading-series.template]]
    - Make sure you had already followed [[Reading Series|dendron://dendron.handbook/area.product.sop.reading-series]]

### After the release
1. Announce release on discord
   - Add contents of `area.product.release.{date}.reading-series` into `#teatime` channel
     - Add an emoji related to the story
   - Add contents of `area.product.release.{date}.notes` into `#releases` channel
     - Add a `:seedling:` emoji
   - Add contents of `area.product.release.{date}.announcement` into `#announcements` channel
     - Add a `:farmer:` emoji
1. Announce release on twitter
   - Use a format similar to the following:

      ```markdown
      Dendron 0.84 has sprouted 🌱

      - Speed improvements in "Dendron: Show Preview"
      - Pod V2 is now available to use directly from dendron-cli
      - New "Community Teatime" events starting this week
      - Contribute #opensource to good first issues in Dendron code

      https://wiki.dendron.so/notes/qcwfzax4uaqj54evgp8li5y/
      ```

1. Announce release on mastodon
   - Use a format similar to Twitter, but optimized for Mastodon. Threads don't work the same in Mastodon, so _don't make a thread._ It's a one message kind of deal. You can always send a second message (such as upcoming events) at another time.
   - Example format with slight modifications to above:

      ```markdown
      Dendron 0.84 #release has sprouted 🌱

      - Speed improvements in "Dendron: Show Preview"
      - Pod V2 is now available to use directly from dendron-cli
      - New "Community Teatime" events starting this week
      - Contribute #opensource to good first issues in Dendron code

      #dendron #vscode #vscodium

      https://wiki.dendron.so/notes/qcwfzax4uaqj54evgp8li5y/
      ```
1. Release the newsletter updates via [[Weekly Newsletter|dendron://dendron.handbook/area.growth.sop.weekly-newsletter]]

## Checklist
![[dendron://dendron.handbook/area.product.sop.weekly-release-notes.checklist]]

## Templates
<!-- Any additional templates (eg. release notes) that might be used -->

### Release 
Weekly release notes are ready in dev. Add an 👍 if all looks good

[^site]: [[Repos|dendron://private/s.github.ref.repos#^T8kaEVtPEEBC]]
[^blog]: [[Repos|dendron://private/s.github.ref.repos#^02M2XTWZQhKm]]
