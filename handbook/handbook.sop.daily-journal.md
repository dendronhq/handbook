---
id: f143773d-3f97-4dbd-8518-603fbb3b0288
title: Daily Journal
desc: ''
updated: 1623669603545
created: 1623165719449
---
## Summary

The daily journal is how we do standup. Instead of a synchronous daily meeting, we do asynchronous journal notes. 

We use the following [[template|templates.standup]] for people's daily journals. 

A daily journal is located at `user.{username}.journal.{date}`.

Daily journals for the current day should be filled out by 5PM local time. A daily journal for the next day should also be created at the same time. For the weekend, make sure that the journal for Monday is ready EoD Friday. 

## Details

A daily journal has the following sections

- discussion
- do
- routine

Note that your daily journal can have additional sections and customizations but the above is the minimum that we recommend. 

### Discussion

This is for anything that you want to bring up for standup

- if you want feedback from a specific team member, `@` mention their username in the discussion
- users can respond to discussions by creating a scratch note and creating a link to the journal note
- you should ping the individual in discord if you've responded to a discussion  (don't forget to sync the workspace first)

#### Example

- user.kevin.journal.2021.06.07

```markdown
## Discussion
- swag item updates
```

- some scratch note created by @kpats

```
- comments for [[user.kevin.journal.2021.06.07.md]]

- swag item updates
> We are shipping everyone oak seeds
```

### Do

This is for things you want to do for the day. The format of this section is described [[here|handbook.sop.todos]]

### Routine

This is for tasks you should do by the end of everyday. 

A common task here is to: 
- Check on the [[weekly journal|handbook.sop.weekly-journal]] for tasks. This also has the nice side-effect of backlinking all weekly journals to the relevant daily journals.

This is for you to customize. Depending on your role, this is different for everyone. We encourage you to create your own template at `templates.standup.{user}` and use that for your daily journals.


