---
id: 27fd4443-58b5-4fdc-a1ca-1aa4ca9f8397
title: Early Seed Release
desc: ''
updated: 1646957443427
created: 1623344680534
---

## Summary
How we handle Dendron's early seed releases

## Steps

### Code

#### Before the release
1. Go to [Create Release Image Github Actions Pipeline](https://github.com/dendronhq/dendron/actions/workflows/create-release-image.yml) and view the latest pipeline run. See [[Pipelines for General Release|dendron://dendron.docs/dev.build.automation#pipelines-for-general-release]] for more info.
1. Install the .vsix file locally and do a sanity check in `test-workspace` 
    - make sure early seed features don't have any obvious bugs
    - See [here](https://stackoverflow.com/questions/42017617/how-to-install-vs-code-extension-manually) for how to install `.vsix` manually
    - If a bug is detected, ping `@Dendron Team` and relevant parties to get it fixed 
1. If everything works, add to the release note thread of the week 

### Docs
1. Make sure [[Early Seed Changelog|dendron://dendron.dendron-site/changelog.early-seed]] is updated by following the process [[here|dendron://dendron.handbook/area.product.sop.changelog-update]]. This should be submitted as a PR to `dendron-site`.
1. When the code is ready, merge into master
    ```sh
    git checkout master
    git pull
    git merge dev
    git push
    ```
1. Check that the changes have made it to the main page
1. Use the following template[^1] to write the announcement message
    - You can see an example of a past announcement [here](https://discord.com/channels/717965437182410783/771518214558449685/878434754918228031)
    - see the sop on release highlights [^4] for release format
1. Announce announce the release in the `#environmentalist` channel with the `@Environmentalists` mention.

## Checklist
- code
    - [ ] test early seed build
    - [ ] if any issues detected, check in changes into the `release/*` branch directly

- docs
    - [ ] [[Early Seed Changelog|dendron://dendron.dendron-site/changelog.early-seed]] is updated
      - [[Changelog|dendron://dendron.dendron-site/templates.changelog]]
    - [ ] changelog is published
    - [ ] announcement made
      - [[Discord Announce|dendron://dendron.handbook/area.product.sop.early-seed-release.temp.discord-announce]]
      - Announce in the `#environmentalist` channel

## Templates

- [[Changelog|dendron://dendron.dendron-site/templates.changelog]]
- [[Discord Announce|dendron://dendron.handbook/area.product.sop.early-seed-release.temp.discord-announce]]

### Good Release

Tests run on early seed, we're ready to ship 🌱

## Reference

### Release Schedule 

Refer to the [Dendron Release Google Calendar](https://calendar.google.com/calendar/u/1?cid=Y19jcjFwNnNhOHUzYzgzY2Q4ZTR0dmd1ZHU3NEBncm91cC5jYWxlbmRhci5nb29nbGUuY29t) for times of Notable events such as Branch Snaps, Target Release Times.


[^1]: [[Template|dendron://dendron.handbook/area.product.sop.release-highlights.template]]
[^2]: [[Update Changelog|dendron://dendron.dendron-site/changelog]]
[^3]: [[Team Announce|dendron://dendron.handbook/area.product.sop.early-seed-release.temp.team-announce]]
[^4]: [[Release Highlights|dendron://dendron.handbook/area.product.sop.release-highlights]]
