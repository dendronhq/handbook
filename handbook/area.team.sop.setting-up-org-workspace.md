---
id: e2t813d635281utz0u4d4df
title: Setting up Org Workspace
desc: How to setup org workspace
updated: 1649698668389
created: 1649698550726
---

## Summary
{{{fm.desc}}}

## Prerequisites
- be part of [[Dendron Github Team|dendron://private/ext.github.teams]]

## Steps
1. If you currently have work in another workspace, make sure to sync your changes by running workspace sync.
1. Clone org-workspace
    ```sh
    git clone git@github.com:dendronhq/org-workspace.git
    ```
1. Open up your Dendron workspace
    - NOTE: we're using `code` CLI in this example but this will vary depending on what VSCode client you use. you can also double click on `dendron.code-workspace` file 
    ```sh
    cd {workspace}
    code .
    ```
1. You will see a prompt to `Open workspace file` on the bottom right corner. Click on the prompt
1. Wait ~30s for your workspace to initialize. Dendron is initializing your workspace and downloading company documents at this point
    - NOTE: if this fails, make sure that you've setup your [[ssh key|dendron://dendron.handbook/handbook.people.onboarding#^bccdwxblcj2u]]
