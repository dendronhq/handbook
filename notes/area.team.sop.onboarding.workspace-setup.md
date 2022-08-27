---
id: rksmggt0kaoi2lapn88rx32
title: Setup your Dendron Workspace
desc: 'The Dendron workspace represents the shared organizational knowledge of our organization. It is managed using Dendron'
updated: 1661573084014
created: 1652308575925
---

## Summary

{{fm.desc}}

## Prerequisites
1. Accept invitation to dendronhq github org (you should get a notification on Github)
    - IMPORTANT: do this before proceeding 
1. Setup a ssh key with your github account. See instructions [here](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) ^bccdwxblcj2u


## Steps
1. Clone the Dendron workspace.
    - If you are currently doing our trial or internship, this will be ![[dendron://dendron.handbook/ext.github.repo.org-trial-ws]]
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
    - NOTE: if you are having trouble setting this up, make sure that you have a [[ssh key|dendron://dendron.handbook/area.team.sop.onboarding.initial-setup#^bccdwxblcj2u]] associated with your github account
1. Wait ~30s for your workspace to initialize. Dendron is initializing your workspace and downloading company documents at this point
    - NOTE: if this fails, make sure that you've setup your [[ssh key|dendron://dendron.handbook/area.team.sop.onboarding.initial-setup#^bccdwxblcj2u]]
