---
id: j60zga2igujjmzri96mr8q5
title: External Resource
desc: ''
updated: 1650308700046
created: 1647744424115
---

## Summary
- #stage.seed

The [[ext]] hierarchy contains [[Proxy Notes|dendron://dendron.docs/rfc.38-links-to-non-note-files#proxy-notes]] to external resources - mainly, links to resources within the various [[Services|dendron://dendron.handbook/s]] that we use as a company.

## Schema
See [[seeds/dendron.handbook/handbook/ext.schema.yml]]

A resource category is described by: `ext.{service}.{category}`
A resource is described using the following path: `ext.{service}.{category}.{resource}`
Resources with subresources are described as follows: `ext.{service}.{category}.{resource}.{subresource}`

- Example: [[Dendron Discord Server|dendron://private/ext.discord.server.dendron]]

## Templates
When creating an entry in the external resource hierarchy, you can use the following [[Template|dendron://private/ext.template]]

## Context
This hiearchy exists to provide stable links to resources that we refer to inside of other notes. This has the following benefits:
- each link becomes a note and now becomes accessible via lookup, backlinks, and the full scope of Dendron's functionality
- its much easier to a resource by its hierarchy then the raw url 
- if the underlying url changes, we juts need to change the url in one place