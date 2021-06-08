---
id: 09a34445-345d-42c9-b82b-6f6691aed668
title: Onboarding
desc: ""
updated: 1623123840979
created: 1618789330639
---

## Summary

The following describes what onboarding at Dendron looks like

## Checklist

- [ ] send discord and github information
- [ ] setup your workspace
- [ ] go over company notes
- [ ] go over the yearly, weekly, and daily hierarchies
- [ ] pick up a first task

## Information

We need your github handle and discord handle to add you to our workspace and community. If you do not have accounts, please create one and message `kpats@` with the details. Once you've got access, you can proceed to the following steps.

## Setting up your workspace

1. Clone the dendronhq workspace: `git@github.com:dendronhq/org-workspace.git`

   - this will pull down two more vaults
     - org-private: company specific things (eg. standup, priorities, etc)
     - org-dev: dev specific things (eg. deployment, qa, operations, etc)
   - you can see what we've been working on under `user.{name}.journal.*` hierarchies

1. Use the `Vault Add` command to add the following remote vaults
   - endpoint: https://github.com/dendronhq/handbook
   - endpoint: https://github.com/dendronhq/dendron-site
   - NOTE: we currently have to do this because these are [workspace vaults](https://wiki.dendron.so/notes/c6fd6bc4-7f75-4cbb-8f34-f7b99bfe2d50.html#workspace-vault). Dendron doesn't add them automatically from the workspace file
   - NOTE2: this also means that you shouldn't commit anything to the `org-workspace`until this is resolved
1. After adding the remote vaults, use `Configure(yaml)` and change the sync option of `dendron-site` and `handbook` to `noCommit` (see example below)
   ```yml
   - 
     fsPath: repos/handbook/handbook
     name: handbook
     sync: noCommit
   ```
   - NOTE: we need to do this because we want meaningful commit messages for these repositories. Setting them to `noCommit` will prevent [workspace sync](https://wiki.dendron.so/notes/c4cf5519-f7c2-4a23-b93b-1c9a02880f6b.html#workspace-sync) from auto syncing them until you commit your changes.

## Company Values

Take a moment to read the `handbook.company*` notes. Especially the following sections:

- [[Mission|handbook.company.mission]]
- [[Values|handbook.company.values]]

## Getting context

You can get caught up on what we've been working on recently by reviewing the [[weekly|handbook.map#weekly]] hierarchy.

You can see our annual goals as a company in the [[yearly|handbook.map#yearly]] hierarchy.

You can also look at individual [[user|handbook.map#user]] hierarchies to see each person's day to day tasks.

This would also be a good time to start your own user.<name> hierarchy. If you have an email alias w/ Dendron, that would be good to use. If not, feel free to pick any name that doesn't conflict with someone's existing note.

- [ ] Create your user.\*.journal.daily hierarchy

## Doing your first task

At this point, you can get started by picking off a good first task from our backlog. You can find our coding guidelines, how to setup Dendron and a list of good first tasks [here](https://wiki.dendron.so/notes/81da87be-2d4e-47b5-a1d6-c0d647e1ab00.html).

- [ ] Add the details of your first task to your daily journal so you can take notes/ask for help etc.

## Workflow

Use the `Dendron: Workspace: Sync` command (command bar + Dendron: Workspace Sync) to keep your repository up to date.

### Merge Conflicts

When you run `workspace sync`, you might get a merge conflict since others could have edited the file. This is expected and use your best sense when resolving the merge conflict.

The typical workflow:

```sh
dendron workspace sync # or Dendron: Workspace: Sync in VSCode
# discover merge conflict
# fix merge conflict
# run the following on the bad file
git add <FILE>
git rebase --continue
# re-run sync
dendron workspace sync
```

## Next Steps

- Make sure you have access to the code: [[Code|dendron://private/pro]]
- Now that you have access to the company vaults, copy the [[Checklist |handbook.people.onboarding.checklist]] over to your own user.<alias> hierarchy and get started on that.
