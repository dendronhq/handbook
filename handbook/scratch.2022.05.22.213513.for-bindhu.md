---
id: 3gmsor8332livibie5abthk
title: For Bindhu
desc: ''
updated: 1653269760098
created: 1653269723969
published: false
---

## Relevant Links
- [[Monday Discord Thread|dendron://dendron.handbook/area.product.sop.weekly-release-notes.temp.discord-thread-start]]
- [[Tuesday Release Changelog|dendron://dendron.handbook/area.product.sop.changelog-update]]
- [[Tuesday Release Notes + Announce|dendron://dendron.handbook/area.product.sop.weekly-release-notes]]
- [[Thursday Discord Thread|dendron://dendron.handbook/area.product.sop.early-seed-release.temp.discord-thread-start]]
- [[Friday Release|dendron://dendron.handbook/area.product.sop.early-seed-release]]
- [[Friday Announce|area.product.sop.early-seed-release.temp.discord-announce#^dw8qj8srmfo2]]


## Weekly Release Calendar
### Monday - Weekly Start
#### Discord
1. Create Discord thread named `weekly-release-{date}` in `#dendron-team` following [[this template|dendron://dendron.handbook/area.product.sop.weekly-release-notes.temp.discord-thread-start]] around 8-10 PM PDT.

#### vault/dendron-site
**Changelog**
1. Update `changelog.md` with information in the weekly journal corresponding to the upcoming Tuesday (in `vault/org-private`).
- Add new entry with the correct version number, and relevant `features`, `enhancements` and `fixes`.
- follow specified format for bullets in [[Changelog Update|dendron://dendron.handbook/area.product.sop.changelog-update]]
**Release Notes**
- Update `changelog.release.{date}` according to [[Weekly Release Notes|dendron://dendron.handbook/area.product.sop.weekly-release-notes]]

### Tuesday - Weekly Release
1. Integrate new updates into blurbs or bullets (bullets from the `weekly journal`, highlight blurbs sent over Discord or drafted)
2. Look at the [dendron-site PRs](https://github.com/dendronhq/dendron-site/pulls) to see if any new documentation has been added to the wiki
3. Follow [[Weekly Release Notes|dendron://dendron.handbook/area.product.sop.weekly-release-notes]]
4. Ask Kevin for review
5. On approval, merge into dev branch
6. Merge into main branch and announce

### Tuesday - Announcements
#### Discord
#### Twitter
- come up with a few bullets to describe the release
- follow template in [[Weekly Release Notes|dendron://dendron.handbook/area.product.sop.weekly-release-notes]]
#### Mastodon
- same as Twitter
- follow template in [[Weekly Release Notes|dendron://dendron.handbook/area.product.sop.weekly-release-notes]]
#### Buttondown Newsletter
- follow [[Weekly Newsletter|dendron://dendron.handbook/area.growth.sop.weekly-newsletter]]

### Thursday - Early Seed Start
#### Discord
1. Create Discord thread named `early-seed-{date}` in `#dendron-team`
following [[this template|dendron://dendron.handbook/area.product.sop.early-seed-release.temp.discord-thread-start]] around 8-10 PM PDT.

#### vault/dendron-site
1. Update `changelog.early-seed` according to [[Early Seed|dendron://dendron.handbook/area.product.sop.early-seed-release]]

### Friday - Early Seed Release
#### vault/dendron-site
1. Integrate new updates into blurbs or bullets (bullets from the `weekly journal`, highlight blurbs sent over Discord or drafted) into `changelog.early-seed`
2. Look at the [dendron-site PRs](https://github.com/dendronhq/dendron-site/pulls) to see if any new documentation has been added to the wiki (decide whether it should be merged in for the release)
3. Await approval from Kevin
4. Upon approval, merge the PR into the `dev` branch
5. Merge into main and announce

### Friday - Announcement
#### Discord 
1. In `#environmentalist` channel, follow [[Discord Announce|area.product.sop.early-seed-release.temp.discord-announce#^dw8qj8srmfo2]]
