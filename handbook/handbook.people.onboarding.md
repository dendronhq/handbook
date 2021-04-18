---
id: 09a34445-345d-42c9-b82b-6f6691aed668
title: Onboarding
desc: ''
updated: 1618789527250
created: 1618789330639
---

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
1. After adding the remote vaults, use `Configure(yaml)` and change the visibility of `dendron-site` and `handbook` to `private` (see example below)
    ```yml
        -
            fsPath: repos/handbook/handbook
            name: handbook
            visibility: private
    ```
    - NOTE: we need to do this because we want meaningful commit messages for these repositories. setting them to private will prevent [workspace sync](https://wiki.dendron.so/notes/23a1b942-99af-45c8-8116-4f4bb7dccd21.html#sync) from auto syncing them