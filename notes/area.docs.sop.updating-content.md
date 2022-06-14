---
id: ptwe0bkvo5c5nwog5v66yr6
title: Updating Content
desc: 'How to update content inside the team workspace'
updated: 1654109352054
created: 1654108798016
---

When updating content in the dendron workspace, policy is different if you are updating a public or private vault

## Updating a private vault
The policy of updating a private vault is straightforward - make any edits and then run [[Workspace Sync|dendron://dendron.handbook/area.team.t.basics.ref.commands#workspace-sync]]. 

If you are creating or updating a SOP, run a sync before and after you change the sop and post the change as an update in [[Daily Asyncs|dendron://dendron.handbook/area.team.sop.daily-asyncs]]

## Updating dendron-site
When you are updating content from dendron-site, make a pull request against the `dev` branch for any changes.
Changes from `dev` are synced every tuesday and friday back with the `main` branch.

## Updating any other public vault

When updating any other public vault that is not `dendron-site`, changes can be submitted as a pull request directly against the `master` branch

## Reference
- [[All Vaults|dendron://dendron.handbook/area.common.ref.vaults]]


[^public] [[Public Vaults|dendron://dendron.handbook/area.common.ref.vaults#public-vaults]]