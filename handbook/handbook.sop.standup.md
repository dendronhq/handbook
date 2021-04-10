---
id: eefd546b-96ee-4830-b11e-dbb1f112a857
title: Standup
desc: ''
updated: 1618029387900
created: 1617592791260
---

- everone should have a `user.{username}` hiearchy, preferably as a standalone vault
- users enter a journal entry for the day's work in the following format

```md
## Discuss
<!-- Anything that you want to bring up during standup -->

## Done
<!-- Anything that was done the day before -->

## Do
<!-- Anything that will be done today -->

## Other
<!-- Anything that comes up -->
```

- the team lead is responsible for creating the standup note for the next day
    - currently, we are doing this as `standup.journal.*` hierarchy
    - once Dendron gets bigger, we will divide this into `team.standup.journal.*`
- template for standup
    - `standup.journal.2021.04.01`

```md
## Standup
![[dendron://user-kevin/user.kevin.journal.2021.04.01]]
![[dendron://user-kpats/user.kpats.journal.2021.04.01]]
## Notes

```
- during standup, one person should be responsible for taking notes
- useful to use something like [gitduck](http://gitduck.com/) to screen share and go over priorities
- after standup, notes should be committed and standup notes for the next day should be created
