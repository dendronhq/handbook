---
id: 3j8f1e2teu9hea2vq56slkb
title: Setup Codespaces
desc: ''
updated: 1651788656728
created: 1651788115455
---

### setup codespaces
1. go to https://github.com/dendronhq-core/dendron
1. create a code spaces that boots up using this setting: https://www.loom.com/i/810cb21bbfdf4f438cc310c0fe026ff6
    - select region to be close to where you are
    - choose 4core CPU
1. this should launch you with vscode with code spaces
1. downgrade the node version to v16 (the default is v17 which causes issues with some of our dependencies)
    ```sh
    nvm install 16
    ```
1. go through installation instructions: [[Dendron Plugin Quickstart|dendron://dendron.docs/pkg.plugin-core.quickstart]]

- NOTE: dendron will be located in `/workspaces/dendron/dendron-main.code-workspace`

### development

same process as local with the following caveats.

- since you are working on a fork of dendron, make sure to fetch from upstream before working on a feature or rebasing to get the latest changes
    - https://www.loom.com/i/d42aa16aef214cc2bb024b1e513401a5
- to create a feature branch, push to a new branch then
    - visit the website of the fork at https://github.com/dendronhq-core/dendron
    - click "create pull request" which will create a PR back to the original repo

### a note on memory

you might run out of memory when working with codespaces. 
instead of running all packages, modify the following to only watch packages you are using.

```sh
npx lerna run watch --parallel 
    \ --scope @dendronhq/common-all 
    \ --scope @dendronhq/common-server 
    \ --scope @dendronhq/engine-server 
    \ --scope @dendronhq/plugin-core 
    \ --scope @dendronhq/dendron-cli 
    \ --scope @dendronhq/pods-core 
    \ --scope @dendronhq/api-server
    \ --scope @dendronhq/dendron-next-server
    \ --scope @dendronhq/common-test-utils
    \ --scope @dendronhq/engine-test-utils
    \ --scope @dendronhq/bootstrap
```

you can use the same technique to only build packages after they have been modified
```sh
npx lerna run build --parallel 
    \ --scope @dendronhq/common-all 
    \ --scope @dendronhq/common-server 
    \ --scope @dendronhq/engine-server 
    \ --scope @dendronhq/plugin-core 
    \ --scope @dendronhq/dendron-cli 
    \ --scope @dendronhq/pods-core 
    \ --scope @dendronhq/api-server
    \ --scope @dendronhq/dendron-next-server
    \ --scope @dendronhq/common-test-utils
    \ --scope @dendronhq/engine-test-utils
    \ --scope @dendronhq/bootstrap
```