---
id: MDqYxBszVoWxNJUZ1C1PE
title: Changelog Update
desc: ''
updated: 1647909158930
created: 1634137544355
---


## Summary
<!-- What is this SOP about -->
Goes over updating the [[Changelog|dendron://dendron.dendron-site/changelog]] and the [[Early Seed Changelog|dendron://dendron.dendron-site/changelog.early-seed]].

## Details

With every release, the [[Changelog|dendron://dendron.dendron-site/changelog]] expands to include the following types of updates (with docs links, when applicable):

- Features
- Enhancements
- Fixes
- Breaking Changes
- Deprecation Notices

### General Format

Changelog format should look like the following:

```markdown
- feat(vaults): early implementation of self contained vaults ([[docs|dendron://dendron.dendron-site/dendron.topic.vaults.self-contained]]) (#2517) @kaan
```

Broken down:

- **feat**: This is a feature. The first part specifies whether this is a feature, enhancement, or fix (`feat|enhance|fix`).
- **(vaults)**: This change is related to Dendron vaults. This section specifies what component of Dendron is changing (`(vaults|publishing|workspace|pods|sync|etc.)`. 
- **early implementation of self contained vaults**: Short description of the change/PR/commit.
- **docs link**: Features should always have a docs reference, and most enhancements should too. Link to the target docs, and link to a specific header when necessary. Format: `([[docs|dendron://dendron.dendron-site/target.note#header]])`
- **(#2517)**: This is the PR number of the change in the Dendron GitHub repository.
- **`@kaan`**: The contributor. If they are not a member of the Dendron team, then this should instead be a Markdown link to the contributor's GitHub profile.

### Breaking Changes and Deprecation Notices

- **Breaking Changes**: This section should point out what functionality is breaking and how to migrate/update their configurations in order to work with the latest version of Dendron. This section should also point out whether the CLI or the Dendron extension (or both) are impacted. Link to docs where able.
- **Deprecation Notices**: This section should point out what older functionality is no longer supported in Dendron, along with directions on how to migrate. Link to docs where able.

### Example

Here is a mock example that contains all potential sections:

```markdown
## 0.80.0

### Breaking changes

The latest release of Dendron will prompt users to automatically migrate their `dendron.yml` configurations to use the latest publishing configuration. Updated workspace configurations (`version: 5`) won't work with older versions of `dendron-cli`.

If `dendron-cli` is not updated, you will encounter the following error message:

> Cannot find minimum compatible client version. This error should never occur! Please report a bug if you have encountered this.

If running the latest `dendron-cli`, users can optionally migrate their configurations directly from `dendron-cli`:

> `dendron dev run_migration --migrationVersion 0.83.0`

### Deprecation Notices

- deprecate(publishing): Legacy publishing has now been removed from `dendron-cli`. Dendron users that haven't yet migrated from `dendron buildSite` commands must migrate to using the `dendron publish` commands.
  - [[Common commands for Next.js publishing with dendron-cli|dendron://dendron.dendron-site/dendron.topic.publish.cook.common]]
  - [[Upgrade Instructions|dendron://dendron.dendron-site/dendron.topic.publish.migration]]

### Features
- feat(vaults): early implementation of self contained vaults ([[docs|dendron://dendron.dendron-site/dendron.topic.vaults.self-contained]]) (#2517) @kaan

### Enhancements
- enhance(pods): support exporting a note to multiple Airtable destinations ([[docs|dendron://dendron.dendron-site/dendron.topic.pod-v2.ref.builtin.airtable.export]]) (#2582) @Joshi

### Fix
- fix(sync): better error message on `Workspace Add and Commit` (#2552) @joshi
```

## Prerequisites
<!-- Optional, anything that needs to be done ahead of time-->

## Steps

> [Loom recording showing example update to early seed changelog](https://www.loom.com/share/60f9c2918c32433c8f3afb237144b870), up to the submission of a PR

1. Make sure all outstanding [docs prs](https://github.com/dendronhq/dendron-site/pulls) from `dendron-site` are reviewed and merged, especially is they are related to this release.
  - follow [[Community Contributions|dendron://dendron.handbook/area.product.sop.community-contributions]] for any merged PRs, and for any newly opened docs issues in `dendron-site`, `dendron-docs`, or other docs-related repos
1. Sync your workspace
1. Create a new branch from the `dev` branch of `dendron-site`, as we want to create a PR (ex. `git checkout -b early-seed-085` or `git checkout -b release-085`)
1. Go to the [[Changelog|dendron://dendron.dendron-site/changelog]] if a production release, or go to the [[Early Seed Changelog|dendron://dendron.dendron-site/changelog.early-seed]] if early seed
1. Update the changelog using [[Changelog|dendron://dendron.dendron-site/templates.changelog]] template
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
    - NOTE: each commit should adhere to our [[commit style|dendron://dendron.docs/dev.process.review#commit-style]] 
    ![[dendron://dendron.docs/dev.process.commit#^pjL1YxpWRgtT:#*]]
1. For changes that are introducing new functionality, make sure that docs are provided at the end of the commit
    - NOTE: if no docs are available, please ping the developer (their alias should be at the end of the alias)
    - in general, all `feat` items and most `enhance` items should have docs
    - eg.
    ```md
    - feat(publish): add `dendron publish dev` command ([[docs|dendron://dendron.dendron-site/dendron.topic.publish.cli#dev]]) (#1238) @kevin
    ```

## Checklist
<!-- Should be used to do the task -->
