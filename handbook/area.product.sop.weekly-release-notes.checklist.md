---
id: QQrTHByWsKowoTEgRxP4M
title: Checklist
desc: ''
updated: 1647025211227
created: 1635724868472
---

### Day Before Release

- [ ] Create Draft PR that includes:
  - [ ] New Dendron Reading Series (`dendron.events.reading-series.yyyy.mm.dd`)
    - [[Reading Series SOP|dendron://dendron.handbook/area.product.sop.reading-series]]
  - [ ] Update [[Changelog|dendron://dendron.dendron-site/changelog]]
    - [[Changelog Update SOP|dendron://dendron.handbook/area.product.sop.changelog-update]]
    - [[Changelog Template|dendron://dendron.dendron-site/templates.changelog]]
  - [ ] New Weekly Release Notes (`changelog.release.yyyy-mm-dd`)
    - [[Weekly Release Notes SOP|dendron://dendron.handbook/area.product.sop.weekly-release-notes]]
    - [[Release Highlights SOP|dendron://dendron.handbook/area.product.sop.release-highlights]]
- [ ] Notice given to team of upcoming release
  - [[Discord Thread Start|dendron://dendron.handbook/area.product.sop.weekly-release-notes.temp.discord-thread-start]]

### Day Of Release

- [ ] Add contributors information to PR once finalized and formatted by team
- [ ] Address any review feedback in PR
- [ ] PR approved, merged to `dev`, and `dev` is merged to `master` (in `dendron-site`)
- [ ] Verify website is updated with latest content

### Announcements After Release

- [ ] Discord
  - [ ] `#teatime`: [[Reading Series|dendron://dendron.handbook/area.product.sop.reading-series]] with `@ServerNotify`
  - [ ] `#releases` post with `@everyone`
    - Release highlights
    - `##Highlights`
    - `## Everything Else`
  - [ ] `#announcements` post with `@ServerNotify`
    - Everything under `## Community` except
      - `### Starboard and TIL Highlights`
      - `### Dendron Reading Series`
      - `## Changelog`
    - Replace `### Event Reminders` section with
      ```markdown
      ### Event Reminders

      - Visit our events calendar: https://link.dendron.so/luma
        - This week we have `<event name(s)>`!
      ```
  - [ ] `#publishing`: Add any publishing-related updates to the [[publishing channel|dendron://dendron.dendron-site/community.discord.channels#publishing]] with `@PublishNotify`
- [ ] Twitter announcement
- [ ] Mastodon announcement
- [ ] Schedule [[Weekly Newsletter|dendron://dendron.handbook/area.growth.sop.weekly-newsletter]]
