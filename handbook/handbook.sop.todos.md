---
id: 0292b34e-47eb-4499-8f49-d9891accdb3d
title: Todos
desc: ''
updated: 1629514083695
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

- a: assigned
- w: work in rpgoress
- n: move to next day (usually combined with `make progress` status)
- x: done
- d: dropped 
- .: made progress
- y: pending deployment or verification
- b: blocked
- m: moved 
- l: delegated to someone else


## Examples

```
- [x] foo task <!-- finished task -->
- [d] foo task <!-- not doing task, no longer relevant -->
- [.n] foo task <!-- got to task but not done, moving to tomorrow. note that statuses can be stacked -->
- [m] foo task <!-- did not get to task, moving to backlog -->
```
