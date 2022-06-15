---
id: ebpudfrf6rg5uut75d29lhg
title: Standard Documentation
desc: ''
updated: 1655261204560
created: 1651791209320
documentId: 1DD6ROb22u-BpLeSY_WUlqedMqVCI25wm-gB6EXw0liI
revisionId: >-
  ALm37BW7VAZzSGhBaAheH7CbILKCGcs-bHKa36Lcv6j2ghpsb7cKWc7c9XUmVbA_QnTZWyg2avSgftzVn8h04w
---

## Summary

This leaflet proposes some general guidelines for the Dendron public docs. 

- Goals:
    - make it umnabiguous where to add docs on features and capabilities
    - make it umnabiguous where to find docs on features and capabilities
    - identify gaps in tooling that will make refactoring into and applying the standard easier in future iterations

- Non-goals:
    - every note be 100% the same: we are still iterating on this standard and it will likely change in the future. it is more important we have a standard that people can follow than an XML spec that accounts for every possible permutation of docs

## Concepts
For the purposes of this discussion, howtos/reference/discussions/tutorials refer to the [four types of documentation](https://kevinslin.com/notes/y0swab2mazgi1793kp3v7f7)

### Topic Branch
A topic branch is a feature in Dendron. It is represented using [[dendron.topic]] hierarchy

## Details

There are two areas that this leaflet addresses. 
- the **overall structure** of the docs 
- the **structure for features** 

## Overall Structure of Docs

This leaflet proposes the following changes:

- simplify user guide (less children)
- simplify dendron.* hierarchy to be product related topics 
    - make contribution its own top level hierarchy
- rename "Guides" to "How tos" 

Resulting hierarchhy:

- dendron
    - dendron.quickstart (Getting Started)
    - dendron.user-guide (User Guide)
        - Basic
        - Edit
        - Retrieve and Navigate 
        - ~~Navigation~~ 
            - > fold into Retrieve
        - ~~Organize~~ Structure 
            - > Rename to `Structure (Organization and Format)`
        - ~~Refactoring~~ 
            - > Fold into `Structure (Organization and Format)`
        - Sharing and Syncing
        - ~~Transferring~~ 
            - > Rename to `Sharing and Syncing`
        - Extending
    - ~~dendron.principles~~  
        - > fold into `dendron` home page
    - ~~FAQ~~ 
        - > move under `dendron.resource`
    - ~~dendron.contribute~~
        - > move to `contribute` (becomes top level hierarchy)
    - ~~dendron.guides~~
        - > Rename to `dendron.howtos` (How)
    - dendron.concepts (Concepts)
    - dendron.ref (Reference)
    - dendron.res (Resources)
        - dendron.res.faq
        - dendron.res.troubleshooting
        - dendron.res.support
- contribute 
    - > everything from dendron.contribute gets moved here
- community
- changelog
- careers

## Structure for Features

All features today are added in the form `dendron.topic.{feature}[.{sub-feature}|{sub-component}]`

### Sections

These are headers for features and are directly inside `dendron.topic.{feature}` 

[[dendron://dendron.dendron-site/templates.topic]] (NOTE: link on handbook won't resolve on website, url: https://wiki.dendron.so/notes/ZljuAhFuNWEOUlFtPlC0h)

### Children
These are the children of features and are located in `dendron.topic.{feature}.*` 

[[Top Level Feature|dendron://dendron.dendron-site/dendron.contribute.documentation.tutorial.top-level-feature]] (NOTE: link on handbook won't resolve on website. url: https://wiki.dendron.so/notes/vyjmifzlvu4w85suec4vd6x)