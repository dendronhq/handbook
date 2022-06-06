---
id: vowugfkoktkt2l7tjnd8lyc
title: Merge Conflic
desc: ''
updated: 1654531028862
created: 1654530169122
---

## Summary

Sometimes you'll get a merge conflict when running `workspace sync`

## Video Walkthrough
See https://www.loom.com/share/0b450cbae5514edca231b077f7bf01a0

## Steps
1. Open up the warning message to see which vault has a bad folder
1. Go to the source control pane to find the notes with conflicts and resolve them
1. Run `> Create Terminal` and select the vault with the conflicts
1. Add the notes to git and commit
    ```sh
    git add .
    git commit -m "resolve merge conflict"
    ```
1. Continue the rebase
    ```sh
    git rebase --continue
    ```
1. Check the status. You know you're done when git doesn't say you're still rebasing
    ```sh
    git status
    ```
1. Repeat this process for any vaults that have conflicts
1. Run `workspace sync` again at the end
