---
id: eefd546b-96ee-4830-b11e-dbb1f112a857
title: Daily Update
desc: ""
updated: 1619794096946
created: 1617592791260
---

- everone should have a `user.{username}` hiearchy, preferably as a standalone vault
- users enter a journal entry for the day's work in the following format

```md
## Discussion

<!-- Things you need help with to get unblocked -->

## Do

<!-- Tasks you want to get done today -->

## Routine

<!-- Daily tax/operational load -->

- [ ] check missed discussions
- [ ] file discussions
- [ ] prep for meetings

## Ongoing Projects

<!-- Should be tracked in the proj.* heirarchy. Longer term initiatives -->

## Done

## Comments

<!-- Space for other people to comment on your daily note (mostly on discussion topics) -->
```

- Purely through the written portion of the update, the rest of the team should get a fair idea of what you're working on, whether you're blocked on anything and what you need help on
- the team lead is responsible for creating the standup note for the next day
  - currently, we are doing this as `daily.journal.*` hierarchy
  - once Dendron gets bigger, we will divide this into `team.daily.journal.*`
- template for standup
  - `daily.journal.2021.04.01`

```md
## Daily Update

### Discuss

<!-- Aggregation of individual open discussions -->

## Notes

<!-- Running list of topics/decisions made during standup -->

### Next Steps

<!-- Action items assigned to individuals with due dates -->

### Individual updates

![[user.kevin.journal.2021.04.01]]
![[user.kpats.journal.2021.04.01]]
```

- during the daily update, one person should be responsible for taking notes
- useful to use something like [gitduck](http://gitduck.com/) to screen share and go over priorities
- afterwards, notes should be committed and notes for the next day should be created
