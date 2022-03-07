---
id: 09a34445-345d-42c9-b82b-6f6691aed668
title: Onboarding
desc: ''
updated: 1646674995839
created: 1618789330639
nav_order: 3
---

## Summary

The following describes the onboarding process at Dendron

## Prerequisites
1. [Setup Dendron](https://wiki.dendron.so/notes/678c77d9-ef2c-4537-97b5-64556d6337f1.html) 
1. Accept invitation to dendronhq github org (you should get a notification on Github)
1. Go throught the Dendron Tutorial. When you install Dendron for the first time, you will be taken through a tutorial that walks you over the basics. If you missed it, you can bring it up again by bringing up the [[Command Prompt|dendron://dendron.dendron-site/dendron._ref.command-prompt]] and typing `Dendron: Launch Tutorial`
    - IMPORTANT: do this before proceeding. 
1. Setup a ssh key with your github account. See instructions [here](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) ^bccdwxblcj2u

## Steps

#### Setting Up Your Workspace 
1. Clone the Dendron incubator workspace 
    ```sh
    git clone ssh://github.com/dendronhq/org-workspace-incubator
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

#### Start individual 
1. Your manager should already have setup a hierarchy for you. You can find it by going to `user.{YOUR_ALIAS}`
1. Go to `user.{YOUR_ALIAS}.onboarding` where you'll find further onboarding instructions as well as details about your initial task(s)

