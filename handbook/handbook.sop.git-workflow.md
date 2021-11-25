---
id: tIFX0R6iEvZUGkOJluYo1
title: Git Workflow
desc: ''
updated: 1624323887653
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

1. Make sure there's a [[test|dev.qa#writing-tests]] for the new feature
1. Make sure all the existing [[tests|dev.qa#running-all-tests]] pass 
1. Do a spot check by running your feature with our [[test Workspace|dev.qa#test-workspace]]
1. If your change reflects documentation changes, also submit a PR to [dendron-site](https://github.com/dendronhq/dendron-site) and mention the doc PR link in your current PR


### Creating a pull request

Because we do weekly releases, we like to do a weekly cadence for pull requests as well. Pull requests for next week's release should be in EOD Thursday ([your timezone](https://www.timeanddate.com/worldclock/converter.html?iso=20210625T115900&p1=tz_aoe&p2=234&p3=64&p4=805&p5=102)).

The naming convention for a pull request is similar to that of a commit and takes the format `{category}: {description}`

```
feat: Dendron can now pass the Turing test
```

If your feature is not yet ready, you are encouraged to submit a pull request but mark it as a draft. This lets others comment on the design. If you're part of the core team, this is the standard practice for weekly deliverables.

If its your first pull request to Dendron, watch out for the [CLA](https://en.wikipedia.org/wiki/Contributor_License_Agreement) bot that will ask you to agree to Dendron's CLA

If its your first pull request and you're on our Discord, make sure that Kevin gives you the [[horticulturalist|community.roles#horticulturalist]] role  👨‍🌾👩‍🌾

After you submit your pull request, check the output of our [integration test](https://github.com/dendronhq/dendron/actions) and make sure all tests pass

Optionally, ping `@Dendron Team` in the `#dev` channel of our [discord](https://discord.gg/AE3NRw9) - we usually respond to PRs within 24h


### Merging Changes

Once your feature request has been approved, it will most likely be merged by the person that is reviewing your code. We do a release every Monday which is also when you should expect your feature to be shipped. We also do an early seed release Thursdays/Fridays. If your changes are in before then, they can also be shipped along side the early seed

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
