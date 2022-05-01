---
id: kOs1cuEvqxzur2I9SdYV6
title: Add Additional Vaults
desc: ''
updated: 1641351399719
created: 1628516973812
---


## Summary

This goes over adding the additional vaults to your workspace

## Steps
- NOTE: if you already have non-committed changes in your `org-workspace` repository, please run a `git stash` before you do the following operations and then `git pop` afterwards

### Create a separate branch
1. Branch the workspace repo 
  ```sh
  cd org-workspace/
  git branch -b {username}
  ```
1. Run vault add commands 

### Adding Dendron-Admin

1. Use [[Vault Add|dendron.ref.commands#vault-add]] to add a new remote vault. Enter the properties in [[here|dendron://private/area.team.ref.vaults#properties]]
1. After the workspace has been added, configure your `dendron.yml` and make sure the following line is added as in [[here|dendron://private/area.team.ref.vaults#yaml]]

### Adding Org Incubator

1. Use [[Vault Add|dendron.ref.commands#vault-add]] to add a new remote vault. Enter the following:
  - endpoint: git@github.com:dendronhq/org-incubator.git
  - path: leave default
  - name: incubator
