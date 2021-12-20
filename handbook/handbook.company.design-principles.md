---
id: sc2PcYvs0Y5Pz7BpmHMmk
title: Design Principles
desc: ''
updated: 1639962298275
created: 1639445515947
---

## Summary

Design principles are used to guide product decisions and feature work.

## Principles

### Developer UX

Dendron aims to create a world class developer experience for managing knowledge.

We aim to provide a tool with the efficiency of vim, the extensibility of emacs, and the approachability of VSCode.

#### Goals
1. features are text centric and composables
1. focus on lowering friction for working with your knowledge base
1. optimize for efficiency, speed, and keyboard focused ux
1. come with sane defaults and the ability to customize to your liking
1. support extension along any dimension
1. keeps simple things simple and hard things possible

### Gradual Structure

Dendron works with any level of structure - instead of forcing users to deal with this upfront, we enable the ability to layer on more structure as needed.

Different knowledge bases require different levels of structure - a PKM used for keeping daily journals is different than a company wide knowledge base used by thousands of developers.

#### Goals
1. provide a gradual structuring mechanism for general knowledge 
1. make it easy to ramp structure up and down when needed

### Build on What Exists

Dendron leverages and composes existing components to build out new features instead of inventing from scratch every time. 

This gives users a consistent interface to work with knowledge and acts as a force multiplier in terms of what they are able to do.

#### Goals
1. introduce a small set of powerful primitives which provides the [[80/20|dendron://dendron.handbook/handbook.company.values#8020]] of all dendron functions
1. build new features by extending or composing existing primitives
