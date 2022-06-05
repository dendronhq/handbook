---
id: rksmggt0kaoi2lapn88rx32
title: Setup your Dendron Workspace
desc: 'The Dendron workspace represents the shared organizational knowledge of our organization. It is managed using Dendron'
updated: 1652308922078
created: 1652308575925
---

## Summary

{{fm.desc}}

## Steps
1. Clone the Dendron workspace.
    - If you are currently doing our trial or internship, this will be ![[dendron://private/ext.github.repo.org-incubator]]
    - Otherwise, this will be ![[Org Workspace|dendron://dendron.handbook/ext.github.repo.org-workspace]]
    ```
    git clone {WS_URL}
    ```
1. Open up your dendron workspace
    - NOTE: we're using `code` CLI in this example but this will vary depending on what VSCode client you use. you can also double click on `dendron.code-workspace` file 
    ```sh
    cd {workspace}
    code dendron.code-workspace
    ```
1. Wait ~30s for your workspace to initialize. Dendron is initializing your workspace and downloading company documents at this point
    - NOTE: if this fails, make sure that you've setup your [[ssh key|dendron://dendron.handbook/area.team.sop.onboarding.initial-setup#^bccdwxblcj2u]]
