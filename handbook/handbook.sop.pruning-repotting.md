---
id: Rdo1OcupIPYGNmS0NvMRR
title: Pruning and Repotting
desc: ''
updated: 1644555860726
created: 1644528948663
---


![Plants being pruned and repotted](https://org-dendron-public-assets.s3.amazonaws.com/images/pruning-and-repotting.jpg)

## Summary
This note goes over how and why we _**prune and repot**_ our past notes.

## What is it?

> :bulb: "To gain knowledge, add things every day; to gain wisdom, subtract things every day." - Lao Tzu

- When _**pruning and repotting**_, each team member goes through everything added to the workspace to keep the workspace in order and prioritize our goals.
- We _**prune out**_ notes and ideas in order to promote new growth.
- We _**repot**_ ideas that have grown out of their existing shells to a suitable location where they could thrive.

## Why do we do it?
### 1. Decluttering of the workspace
- **The value of a note diminishes over time** if it cannot be effectively utilized and looked up.
- Removing stale notes and/or refactoring them into a permanent, meaningful piece of information elsewhere is necessary for healthy growth.
    - For Dendron as an organization, the ideal expected outcome of this should be an **actionable project** or an **idea that could be germinated into a future project**.

#### 1.1 Scratch notes
- Scratch notes are a good way to capture the immediacy of ideas but _have little meaning without the context_ in which the scratch notes were created.
- Old scratch notes lose their meaning as time goes by, even if they contain valid and useful information.
    - This is because old scratch notes lose their context as we forget about them, unless we find a proper hierarchy for (or get rid of) them.

> :warning: Having a lot of scratch notes is not by itself a bad idea. If capturing an idea quickly in a larger context of a different note has served its purpose, **there is no need to repot it**. That being said, since scratch notes will most likely be relevant when presented with the accompanying context, it might _introduce noise in a different view_ (e.g. graph view or tree view) where the context is hard to see or is not present. In this case, it's worth **filtering them out** from those affected views.

#### 1.2 Journal notes
- Journal notes are great for organizing tasks and goals in a temporal manner, but as items carry over it creates a lot of duplicates.
- Similar to scratch notes, a massive trail of journal notes may provide little to no utility as they become older and lose their context.

> :warning: Consider keeping journal notes as is and not repotting them into another note. By definition, a journal note captures what happened at a particular point of time. Try to **extract insights** from past journal notes and **fix obvious errors** in them, but keep the general content of the notes intact.

> :warning: Similar to scratch notes, journal notes can potentially introduce noise in other views such as the graph view or tree view. Consider **archiving** them somewhere else once you have extracted meaningful insights from them or if you are certain that you won't be looking them up regularly.

### 2. Retrospection
- Simply writing notes is not enough to cultivate a lively workspace; it is crucial that we carefully observe how our notes grow in order to learn and adapt.
- This goes for the actual content of the notes itself, but also the meta structure of the notes as well.
- Having a pruning session regularly **gives us a chance to look at how our ideas and note grew over time** and iterate on what we did well and what we didn't.

> _**Wouldn't it be better to do retrospection on a project basis?**_
> - Retrospects are a good way to evaluate what has been done well or otherwise.
    - For _mission critical_ matters, consider doing a retrospect _immediately_ after the incident has been resolved.
> - However, it's not clear how often we should do this, and on what basis we should do this (i.e., _appropriate granularity_ and _cadence_ is unclear).
    - By lumping retrospection into a monthly event, we can _ignore the headache of figuring out an appropriate granularity_.
    - The _cadence_ in which we run a pruning / repotting session can be _adjusted based on our needs_.
> - _Impromptu retrospects are hard_ to do with a fully-remote team, and _sporadic retrospects will inevitably cause context switches at unexpected times_ for participants.
    - With scheduled sessions, one could prepare asynchronously _ahead of time_ and also have a _reasonable expectation_ of what work has to be done beforehand.

### 3. Serendipity
- Beneath the overgrown vines there could be a hidden budding flower or a fruit that is waiting to be discovered.
- With notes added to the workspace each day, one's brilliant idea could get buried in the multitude of other notes.
- Regularly pruning out the notes gives us **a chance to discover great ideas** that were hidden.
    - We can then turn these into projects and figure out actionable tasks (repotting).

## Principles

### The 4D's of pruning
1. **Dead**
    - These are notes/ideas that used to have a purpose, but have lost their immediate purpose.
    
    > e.g.) 
    - You have created a note containing documentation for a feature X in the past, but this has become obsolete. This note is considered `Dead`.
    - If this note is not linked in a broader context, you can safely remove this note.

1. **Diseased**
    - Notes that are incomplete, not tended well, or contain wrong information.

    > e.g.) 
    - You have partially created a note to document something. At some point, you have moved onto a new note and finished off the documentation there. Both contain similar content, but one is incomplete. This note is considered `diseased`, and you can safely remove the partial note and correctly link the complete one.
    - You have created a note that turns out to be misleading or wrong. If this note is something that will be potentially looked up later, you can fix the errors. Otherwise, it is safe to delete it.

1. **Damaged**
    - Notes with syntax errors, or malformed frontmatter, missing links, etc.

    > e.g.) 
    - You have a syntax error in the frontmatter (like a trailing comma after a variable)
    - You have a note that has one less or one extra square bracket for a wikilink. This will cause some problems with parsing later on and should be fixed.

1. **Deranged**
    - These are notes/ideas that contain useful information but are placed in an ill-defined location or otherwise hidden.
    - It may be structured in a way that can't be immediately useful for anyone.
    - Somehow the note/idea is incomplete or out of context.
    - Notes that are obstructed by other content or are obstructing other notes.

    > e.g.) 
    - You were in a pinch, so you copy-pasted a long stack trace inside your journal note at some point rather than dumping them in a scratch note. This could obstruct the meaningful content in that journal note and should be removed or refactored into a separate note.
    - You had a Eureka moment and jotted down an idea to make Dendron even better. However, you were in a meeting and this idea was written in your meeting notes. This should be repotted to a place where you keep your ideas, or turned into a `proj.*` item.
