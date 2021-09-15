---
id: 09a34445-345d-42c9-b82b-6f6691aed668
title: Onboarding
desc: ''
updated: 1631728479689
created: 1618789330639
nav_order: 3
---

## Summary

The following describes the onboarding process at Dendron

## Process

### Prerequisites
1. Send Kevin your github information
1. [Setup Dendron](https://wiki.dendron.so/notes/678c77d9-ef2c-4537-97b5-64556d6337f1.html) 
    - NOTE: we recommend using [VSCode Insider](https://code.visualstudio.com/insiders/) as your Dendron Client and regular [VSCode](https://code.visualstudio.com/) for development work
1. Get permission to join the github workspace (you should get a notification on Github when this is ready)

### Steps

#### Setting Up Your Workspace 
1. Clone the Dendron private workspace (this will be sent to you by email)
    ```sh
    git clone {workspace-url}
    ```
1. Open up your Dendron workspace
    - NOTE: we're using `code-insider` CLI in this example but this will vary depending on what VSCode client you use
    ```sh
    cd {workspace}
    code-insdier .
    ```
1. You will see a prompt to `Open workspace file` on the bottom right corner. Click on the prompt
1. Wait ~30s for your workspace to initialize. Dendron is initializing your workspace and downloading company documents at this point
1. After your workspace is finished initializing, you should have a workspace with the following vaults (your workspace might look different depending if you are full time or still in the trial period)
![[handbook.map#vaults,1:#*]]

#### Go Over Company Values
1.  Take a moment to read the `handbook.company*` notes. Especially the following sections:
  - [[Mission|handbook.company.mission]]
  - [[Values|handbook.company.values]]

#### Get Context on whats been happening
1. Read up on company [[schemas|handbook.map#schemas]] to understand how to navigate the workspace
1. Look at [[Projects|schemas.proj]] to see what the current month's initiatives are as well as whats coming up
1. Review the [[Weekly|schemas.weekly]] notes to see progress we've made over the past few weeks (you can go all the way back to week 1)
1. Review [[daily journals|schemas.user#dailyjournal]] to see what a typical day at Dendron is like

#### Get ready to build the future of knowledge management
1. Your manager should already have setup a hierarchy for you. You can find it by going to `user.{YOUR_ALIAS}`
1. Go to `user.{YOUR_ALIAS}.onboarding` where you should have a copy of our [[Onboarding checklist|templates.people.onboarding]] to walk you through the rest of the process
