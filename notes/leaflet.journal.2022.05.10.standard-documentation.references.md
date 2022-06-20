---
id: eqaq8kybv2t7ko1e9xou37p
title: References
desc: ''
updated: 1655764501301
created: 1654788092175
---

## Summary

This covers the references section of [[Standard Documentation|dendron://dendron.handbook/leaflet.journal.2022.05.10.standard-documentation]] in more detail.

## Concepts

### Refs
For the purposes of this note, a ref is anything that fits under `dendron.roebe comprehensivcef`. Examples:
- cli
- config
- commands
- apis

## Structure of References
- there should be an individual note for each ref
    - eg: [[nav_order|dendron://dendron.dendron-site/dendron.topic.sidebar.tree-view.config.nav_order]]
- refs should be children ot the corresponding topic branch [^topic]
    - eg. `[[dendron.topic.template.config]]`
- if a topic branch has subcomponents, then the ref should be the child of the closest matching subcomponent
    - eg. [[nav_order|dendron://dendron.dendron-site/dendron.topic.sidebar.tree-view.config.nav_order]]
- the config that is the direct child of a topic branch should have the index of all configuration for subcompoents as well as the topic
    - eg. `dendron.topic.sidebar.config`
    ```md
    ## Global
    <!-- This affects the topic directly (eg. sidebar configuration -->

    ### Foo
    ![[dendron.topic.sidebar.config.foo]]

    ## Tree View
    <!-- This is the config for the tree view subcomponent. Should be a note ref-->
    ![[dendron.topic.sidebar.tree-view.config]]

    ...
    ```
- [[dendron.ref.config]] should contain the index of all configuration, grouped by topic 
    ```
    - ...
    - [[dendron.topic.lookup.config]]
    - [[dendron.topic.sidebar.config]]
    - ...
    ```

## Additional Thoughts
- in an ideal world, we can define the ref in one place and programatically generate the configuration indexes elsewhere 
    - in the above example, we would add a config once in `dendron.topic.sidebar.tree-view.config.nav_order`
    - dendron should be smart enough to then include it in `dendron.topic.sidebar.config`, `dendron.topic.config`, and `dendron.ref.config` as needed
    - because we don't have this today, we are manually adding it in
    - in the future, we should be able to embed these sections using [[22 Queries|dendron://dendron.docs/rfc.22-queries]]


[^topic] : [[Topic Branch|dendron://dendron.handbook/leaflet.journal.2022.05.10.standard-documentation#topic-branch]]
