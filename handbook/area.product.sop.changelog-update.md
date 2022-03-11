---
id: MDqYxBszVoWxNJUZ1C1PE
title: Changelog Update
desc: ''
updated: 1646956819759
created: 1634137544355
---


## Summary
<!-- What is this SOP about -->
Goes over updating the [[Changelog|dendron://dendron.dendron-site/changelog]] and the [[Early Seed Changelog|dendron://dendron.dendron-site/changelog.early-seed]].

## Prerequisites
<!-- Optional, anything that needs to be done ahead of time-->

## Steps

1. Sync your workspace, to ensure on latest `dev` branch of `dendron-site`
1. Create a new branch from the `dev` branch `dendron-site`, as we want to create a PR (ex. `git checkout -b early-seed-085` or `git checkout -b release-085`)
1. Go to the [[Changelog|dendron://dendron.dendron-site/changelog]] if a production release, or go to the [[Early Seed Changelog|dendron://dendron.dendron-site/changelog.early-seed]] if early seed
1. Create a new release using [[Changelog|dendron://dendron.dendron-site/templates.changelog]] template
1. Go to the `Ready to Ship` section of the weekly journal for this week
    - eg. `dendron://private/weekly.journal.2021.10.19`
    - Categories of focus: `Features`, `Enhancements`, `Fix`, and anything related to deprecations or breaking changes. `Internal` is ignored when it comes to the changelog.
1. For each category, copy over everything under the `*** in master` line and copy it to the changelog ^r08juF8Rt8Ds
    - move the lines under `*** in master` below `*** in changelog` after doing this
    - eg. before copying
    ```md
    ...
    ### Enhancements
    - *** in master
    - enhance(publish): support publishing to github as a export template (#1234) @kevin
    - enhance(publish): support `--yes` flag when exporting to skip prompts (#1235) @kevin
    - enhance(publish): initialize template will also install dependencies (#1236) @kevin
    - enhance(publish): warn when `assetsPrefix` isn't set (#1237) @kevin
    - *** in changelog
    ```
    - eg. after copying
    ```md
    ...
    ### Enhancements
    - *** in master
    - *** in changelog
    - enhance(publish): support publishing to github as a export template (#1234) @kevin
    - enhance(publish): support `--yes` flag when exporting to skip prompts (#1235) @kevin
    - enhance(publish): initialize template will also install dependencies (#1236) @kevin
    - enhance(publish): warn when `assetsPrefix` isn't set (#1237) @kevin
    ```
    - NOTE: each commit should adhere to our [[commit style|dendron://dendron.docs/dev.process.commit#commit-style]] 
    ![[dendron://dendron.docs/dev.process.commit#^pjL1YxpWRgtT:#*]]
1. For changes that are introducing new functionality, make sure that docs are provided at the end of the commit
    - NOTE: if no docs are available, please ping the developer (their alias should be at the end of the alias)
    - in general, all `feat` items and most `enhance` items should have docs
    - eg.
    ```md
    - feat(publish): add `dendron publish dev` command ([[docs|dendron://dendron.dendron-site/dendron.topic.publish.cli#dev]]) (#1238) @kevin
    ```
1. Submit PR
1. Depending 

## Checklist
<!-- Should be used to do the task -->
