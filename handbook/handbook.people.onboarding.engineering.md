---
id: c7a2aeaa-f531-4352-a1bc-56504b25a38f
title: Engineering
desc: ''
updated: 1642526428316
created: 1622499448820
---
## Summary

This goes over engineering onboarding. For onboarding, review the follow procedures.

## Your first task

- you should have already been assigned an initial first task when you joined the company 
- setup the dendron monorepo by following instructions [[here|pkg.plugin-core.quickstart]]
- go over our git workflow in [[starting work|dendron://dendron.docs/dev.process.review#starting-work]]
- get a sense of how all the subcomponents work by reading the overal [[architecture|dendron://dendron.docs/dev.arch]]
- get started on your task 
  - schedule a [[pairing session|user.kevin.ref.cal]] with [[Kevin|user.kevin]] sometime in your first week
    - the pairing session can be used to go over any blockers or to simply work on your first task with an extra set of eyes to help

## Development Process

- you can find our style guide [[here|dev.process.code]]
- if your working on a feature, rebase from master after every monday release to minimize chances of merge conflicts
- when testing code, we have a convention of adding "bond" to output values we want to debug - its easy to find in logs but please don't commit as it makes it harder to grep

## Pull Request
- see [[Review|dev.process.review]]

## Getting Help

See [[Getting help for development|handbook.sop.dev-help]]

## Standup
![[handbook.people.onboarding.common#standup,1]]

## Code Review

- we do code review using pull request
- the expectation is that you have a pull request ready by the end of every week
  - pull requests need to be fully complete and can be submitted in `draft` form if notcomplete
  - having pull requests available helps with [[Iterate|handbook.company.values#iterate]] and having others weigh in while a feature is still being worked on

