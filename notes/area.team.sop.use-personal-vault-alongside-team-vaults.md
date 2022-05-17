---
id: kOs1cuEvqxzur2I9SdYV6
title: Use Personal Vault Alongside Team Vaults
desc: ''
updated: 1652757917866
created: 1628516973812
---


## Summary

This goes over how to add a personal vault to the team workspace


## Steps

1. Read about [[Local Config Override|dendron://dendron.dendron-site/dendron.topic.local-config-override]] 

1. Add your personal vault inside the `local/` folder
  - TIP: if you already have a personal vault located elsewhere, you can also symlink it to the `local/` folder

## Example

Sample `dendronrc.yml` file for kevin's private workspace

```yml
workspace:
      -
          fsPath: local/kevin-private
          name: kevin-private
```
