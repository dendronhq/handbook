---
id: 0292b34e-47eb-4499-8f49-d9891accdb3d
title: Todos
desc: ''
updated: 1623348727378
created: 1622146649559
---

## Summary

This goes over how we format todo notes at Dendron.

## Sections
- high: something that should be completed today
- mid: something that can be postponed
- new: something that came up and needs to be prioritized

## Status

This is added to the end of a todo. 


- p: postponed (move to next day)
- `>`: move to next day (usually combined with `make progress` status)
- x: done
- ~: no longer applicable (dropped)
- .: made progress
- y: pending deployment
- v: pending verification
- b: blocked
- m: moved 

Examples
```
- [x] foo task <!-- finished task -->
- [p] foo task <!-- did not get to task, moving to tomorrow -->
- [~] foo task <!-- not doing task, no longer relevant -->
- [.>] foo task <!-- got to task but not done, moving to tomorrow -->
- [m] foo task <!-- did not get to task, moving to backlog -->
```
