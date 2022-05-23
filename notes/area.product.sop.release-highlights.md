---
id: kaSUyUz2IgIio6eNnEmQ7
title: Release Highlights
desc: ''
updated: 1646957499832
created: 1634138438783
---

## Summary
<!-- What is this SOP about -->
This goes over writing release highlights.

## Details

The first sections of any release notes will contain an overview highlighting specific features and enhancements of a release.

This is made up of:

- Overview of features, enhancements, and/or breaking changes of importance in the release.
- `## Highlights`: Changelog items referenced in the overview.
- `## Everything Else`: Changelog items not referenced in the overview.

### Style

```markdown
Dendron <version> has sprouted 🌱

**Highlight type:** Description here.

- More information: [[Title of Docs and Header if Used|dendron://dendron.dendron-site/example.docs]]

**Highlight type:** Description here.

- More information: [Title of Docs and Header if Used](https://docs.dendron.so/)
```

- **Bold** is used to help signify that a different feature/enhancement/breaking/etc. changes.
- Bullet points help break up the highlights.
- If the docs exist outside of `dendron.dendron-site`, then make sure to provide an external link instead (`[label](link target)`). Otherwise, these links will appear as private/broken in the published documentation.
- Add associated changelog items to the `## Highlights` section, and remaining changelog items to `## Everything Else`. Make sure to remove all PR and contributor references. Remove docs links if they are being provided in the highlights overview already.

### Example

Example from [[0.87 Release|dendron://dendron.dendron-site/changelog.release.2022-03-22]]:

```markdown
Dendron 0.87 has sprouted  🌱

**Breaking changes:** We updated the airtableId format to be a dictionary instead of a single value. This makes it possible to export a single note to multiple tables.

If you are using v2 of the airtable pod, you can migrate to the new version by following the [[instructions here|dendron://dendron.dendron-site/dendron.topic.pod-v2.ref.builtin.airtable.migration#migrating-to-0870]].

- More information in the [RFC on standardizing source-field mapping for Pods](https://docs.dendron.so/notes/N0G4s23hFDGVnsjHhh6dt.html)

**Self Contained Vaults:** We are now in early preview of self contained vaults. This lets you use and share your Dendron vaults without the need of a workspace.

If you are interested in trying this out, please fill out this [survey](https://airtable.com/shr0cwk0a9tujeipZ) and we'll add you to early-preview where we'll be holding discussions and offering support. We'll also send you specialized instructions for how to set up self contained vaults!

- More information in [in our RFC about self contained vaults](https://docs.dendron.so/notes/aOOBYTowLEKJDEtLWFiHb/)

**Speed Improvements:** `Dendron: Show Preview` refreshes faster and editing larger workspaces is more responsive.

This release also includes a number of fixes and improvements, including a new command to aid in creating and reading backup files.

- More information [[in our documentation on open backup|dendron://dendron.dendron-site/dendron.ref.commands#open-backup]].

## Highlights
- feat(vaults): early implementation of self contained vaults
- enhance(workspace): faster preview refresh
- enhance(workspace): faster editing in large workspaces
- enhance(internal): provide a standard way to create and read backup files

## Everything Else
- fix(workspace): fix crash that can happen when bad frontmatter is present during doc save
- fix(publish): customHeaderPath breaks publishing if value is set to anything except `header.html`
- fix(basics): ensure note title is always a string to avoid errors
- fix(sync): better error message on `Workspace Add and Commit`
- fix(lookup): lookup (without spaces) should be case-insensitive
- fix(workspace): issue with notes not being saved on export
- fix(workspace): race condition when backing up configuration
- feat(workspace): doctor command to find (and suggest fix for) keyboard conflicts
- enhance(workspace): warn on keyboard conflicts on first install
- enhance(pods): support exporting a note to multiple Airtable destinations
- fix(views): unblock preview rendering when backlink is invalid
- fix(workspace): race condition when loading native workspace
- fix(workspace): prevent errors in Open Backup Command and Run Migration Command in native workspaces
```

## Prerequisites
<!-- Optional, anything that needs to be done ahead of time-->
- make sure [[Changelog Update|dendron://dendron.handbook/area.product.sop.changelog-update]] is already completed

## Steps
1. Use the release highlights template [^1] to announce releases
1. Organize changes into highlights 
    - If highlights have not been pointed out by the team, reach out to the team to confirm what needs to be highlighted.

## Templates

[^1]: Template used for for general releases (ex. `changelog.release.<release>`) [[Weekly Public Announcement|dendron://dendron.dendron-site/templates.release.weekly-public-announcement]]

## Example

- [[Release Notes and Highlights for 0.87 Release|dendron://dendron.dendron-site/changelog.release.2022-03-22]]
