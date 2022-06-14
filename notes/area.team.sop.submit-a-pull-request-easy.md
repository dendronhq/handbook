---
id: o7i52oeoih1fwsoos43dv6h
title: Submit a Pull Request (Easy Mode)
desc: 'Simplified pull request flow'
updated: 1654445724072
created: 1652307349535
---

## Summary

{{fm.desc}}

## Prerequisites

If you are new to git, see [[Git|dendron://dendron.dendron-site/dendron.concepts.git]]

## Quickstart
1. Install the github client > https://desktop.github.com/
1. Add a repository
  - if you are adding a repository that you already cloned, choose **add the existing repository** in the UI  > https://www.loom.com/share/d4f4bd0c7cda499f948aa45a41b72513
  - if you are cloning a new repository, select **clone repository**
  - NOTE: the Dendron team workspace is a composite of multiple repositories. you want to add each one individually 

## Submit a pull request
Video Example: https://www.loom.com/share/429f9cdfa7eb4b728b50e46983ea3e93

1. Make changes in the repository
1. Switch to the github app
1. Create a new branch
  - select take your changes to new branch
1. Commit the changes
1. Publish changes
1. Create a pull request
1. Add reviewers to your pull request
1. IMPORTANT: While your pull request is in review, don't forget to switch back to the main branch to continue working (otherwise, none of your changes will be changed)
1. If you get requests to make changes, switch branches by following [[Making changes to your pull request|dendron://dendron.handbook/area.team.sop.submit-a-pull-request-easy#making-changes-to-your-pull-request]]

## Making changes to your pull request
1. If you get updates on your pull request, switch back to your branch to make any necessary changes 
    - if you were working on something in the main branch, run a `workspace sync` to save the changes
1. Make changes and push to your branch
    - TIP: there's no need to create another pull request at this point

## Merging changes from another branch
See https://youtu.be/UTEHbTO5bnA

## Verify

To make sure you're setup, submit a pull request to [[ext.github.repo.private]] with a new note `[[user.{username}.hello]]` and add @kevin as a PR reviewer

## Checklist
- [ ] create a new branch
- [ ] commit changes to new branch
- [ ] publish branch
- [ ] submit pull request
- [ ] add reviewers to your pull request
- [ ] switch back to the main branch