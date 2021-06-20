---
id: tIFX0R6iEvZUGkOJluYo1
title: Git Workflow
desc: ''
updated: 1624216920883
created: 1624215795020
---

## Summary

How we work with code and git

## Process

We employ the [feature branch workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow) when working with git. 

### Working on a new Feature
This means that every feature will go into a feature branch during local development and pushed to the origin with the same name. When changes are ready to be reviewed, submit a pull request against `master`. 

For feature branches, we use the following conventions:
- feat/{feature-name}
- fix/{fix-name}

### Commit Style
- we follow [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) with the following tags
- categories:
  - feat: feature - introduce new functionality
  - enhance: enhancement - improve existing functionality
  - fix: make something not broken
  - chore: backend improvements
  - spike: not complete commit
 
If you are introducing a breaking change, either add an `!` after the category or a footer at the end of your message

```
feat: allow provided config object to extend other configs

BREAKING CHANGE: `extends` key in config file is now used for extending other config files
```
> Example from [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) licensed under [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/)

```
refactor!: drop support for Node 6
```
> Example from [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) licensed under [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/)

### Pre-Requisites

1. Make sure there's a [[test|dendron.dev.qa#writing-tests]] for the new feature
1. Make sure all the existing [[tests|dendron.dev.qa#running-all-tests]] pass 
1. Do a spot check by running your feature with our [[test Workspace|dendron.dev.qa#test-workspace]]
1. If your change reflects documentation changes, also submit a PR to [dendron-site](https://github.com/dendronhq/dendron-site) and mention the doc PR link in your current PR


### Creating a pull request

Because we do weekly releases, we like to do a weekly cadence for pull requests as well. Pull requests for next week's release should be in 5pm local time on Thursday at the latest. 

If your feature is not yet ready, you are encouraged to submit a pull request but mark it as a draft. This lets others comment on the design. If your part of the core team, this is the standard practice for weekly deliverables.

If its your first pull request to Dendron, watch out for the [CLA](https://en.wikipedia.org/wiki/Contributor_License_Agreement) bot that will ask you to agree to Dendron's CLA

If its your first pull request and you're on our Discord, make sure that Kevin gives you the [[horticulturalist|dendron.community.roles#horticulturalist]] role  👨‍🌾👩‍🌾

After you submit your pull request, check the output of our [integration test](https://github.com/dendronhq/dendron/actions) and make sure all tests pass

Optionally, ping `@Dendron Team` in the `#dev` channel of our [discord](https://discord.gg/AE3NRw9) - we usually respond to PRs within 24h


### Merging Changes

Once your feature request has been approved, it will most likely be merged by the person that is reviewing your code. 

## Checklist

- Pre-Requisites
	- [ ] create a new branch according to our branching convention
	- [ ] implement feature/fix
	- [ ] write test
	- [ ] check existing tests pass
	- [ ] submit documentation pr if relevant
- Creating a pull request (first time)
	- [ ] sign the CLA
	- [ ] ping Kevin about the `horticulturalist` role
- Creating a pull request 
	- [ ] make sure integration tests pass