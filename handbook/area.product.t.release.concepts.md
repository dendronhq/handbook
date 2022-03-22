---
id: 12vr49yakuoly3xqmjgy7i3
title: Concepts
desc: ''
updated: 1647926543864
created: 1647906109890
---

### Changelog

With every release, the [[Changelog|dendron://dendron.dendron-site/changelog]] expands to include the following types of updates (with docs links, when applicable):

- Features
- Enhancements
- Fixes
- Breaking Changes
- Deprecations

Updates are done following a commit-style.

### Highlights



Example:

```markdown
Dendron 0.84 has sprouted  🌱

Speed improvements: `Dendron: Show Preview` should be much faster now because of note sync/image optimization!

Pod V2 Preview features continue growing: `dendron exportPodV2` is now available with `dendron-cli`. Previously, you could only run Pod V2 commands if you were within VS Code / VSCodium, but you can now run exports from the CLI ad-hoc or in scripts.

- More information: [[Pod V2 CLI|dendron://dendron.dendron-site/dendron.topic.pod-v2.cli]]

### Highlights
- feat(pods): support pods v2 in CLI
- enhance(views): faster image preview by using native vscode webview urls
- enhance(views): faster webviews by reducing engine sync operations

### Everything Else
- enhance(views): separate tag configuration for preview and publish ([[docs|dendron://dendron.dendron-site/dendron.ref.config.preview]]) 
- fix(schema): Apply schema template for goto-note-command if template is in different vault
- fix(publish): Table of Contents is missing user tags, inline code, dashes and underlines
- fix(workspace): dendron can hang when trying to provide hover for large non-dendron file
- fix(views): clicking preview links for non-note files
- fix(views): Code blocks and spans in preview are html encoded
- fix(workspace): don't call reload index if action is findIncompatibleExtension
- fix(views): don't refresh tree view if note visible
```

### Early Seed

These are pre-release versions of Dendron extensions made available to [[Environmentalist|dendron://dendron.dendron-site/community.discord.roles#environmentalist]].

- Release cadence: Every Friday

### Release Notes

Release notes are done with the General Release of Dendron that comes out each Tuesday. These provide quite a bit more context compared to the changelog notes, including:

- Feature and enhancement highlights
- Upcoming events
- Discord community messages from the [[today-i-learned|dendron://dendron.dendron-site/community.discord.channels#today-i-learned]] and [[starboard|dendron://dendron.dendron-site/community.discord.channels#starboard]] channels
- Community contributions: contributors that have been raising issues, contributing code, contributing docs, etc. For more information, view the documentation on [[Discord Roles|dendron://dendron.dendron-site/community.discord.roles]]
- General announcements: Blog posts, videos, other events/resources of note, etc.

The release notes also serve as the content submitted to subscribers of the Dendron Newsletter.

### Newsletter

![[dendron://dendron.dendron-site/community#dendron-newsletter,1:#*]]

