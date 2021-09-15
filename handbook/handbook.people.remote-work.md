---
id: zBlxjKJ0bFMcLJXhch2U0
title: Remote Work
desc: ''
updated: 1631727671093
created: 1631220480957
---

## Summary

Remote work comes with lots of flexibility but also introduces challenges in communication and coordination. This goes over some best practices we're experimenting with at Dendron to make the process better.


## Best Practices

### Messaging

When sending messages to team members, the expectations for all messages is that they are async[^async], meaning that the other person has at least **12h** or more to respond. 

If you need to send a synchronous[^sync] message, be considerate of people's hours of availability [^hours] and add a `#sync` after the message. 

```
@kevin the latest release needs to be rolled back because of a bug in lookup #sync
```

Synchronous messages should be reserved for when you need immediate feedback. Some examples of good use cases:

- there's an issue with a feature that is blocking deployment
- there's a critical bug that is actively degrading the Dendron experience
- there's an issue that the current oncall needs to look at during their working hours



## Concepts

### Async

A process that can happen without two or more parties needing to coordinate in real time. Action can be taken when time permits.

### Sync

A process that requires two or more parties to coordinate in real time. Action should be taken immediately.

### Hours of Availability

The combination of time zone and regular work hours as listed in the user [[readme|templates.user-readme#summary]] defines someone's **hours of availability**.



[^hours]: [[Hours of Availability|handbook.people.remote-work#hours-of-availability]]
[^sync]: [[Sync|handbook.people.remote-work#sync]]
[^async]: [[Async|handbook.people.remote-work#async]]