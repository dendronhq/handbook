
## Summary
<!-- What is this SOP about -->
How we communicate in an all remote, async first fashion

## Best Practice

### In General
- If you are sending a message, unless sending during work hours, give people at least **12h** to respond
- If you are receiving a message during the work week, respond within **12h** 

### Messaging

We have 3 priorities for messages.

- async
- priority
- sync

#### async
async messages are not urgent. the recipient has 12h durign work hours to respond. this is the default status of a message unless otherwise marked

#### priority
priority messages are urgent. the recipient should try to respond within 1h of getting this message during work hours. add `#prio` after your message to indicate a priority message

#### sync
sync messages are real time. we almost never use sync messages. add a `#sync` after your comment to indicate a sync message

```
@kevin the latest release needs to be rolled back because of a bug in lookup #sync
```

Synchronous messages should be reserved for when you need immediate feedback. Some examples of good use cases:

- there's an issue with a feature that is blocking deployment
- there's a critical bug that is actively degrading the Dendron experience
- there's an issue that the current oncall needs to look at during their working hours


[^hours]: [[Hours of Availability|handbook.people.remote-work#hours-of-availability]]
[^sync]: [[Sync|handbook.people.remote-work#sync]]
[^async]: [[Async|handbook.people.remote-work#async]]