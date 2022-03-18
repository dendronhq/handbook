---
id: q2o6Aggu8kZuiIur6RFgq
title: Project Management
desc: ''
updated: 1644780101188
created: 1641419782227
---


## Summary
This goes over how to work with [[Projects|dendron://private/area.team.ref.projects]]

## Prerequisites
- have access to the following pod config: [[pods/custom/config.dendron.projects.yml]]
- TIP: add the following to your keyboard binding to quickly export a project
```json
    {
        "key": "cmd+k p",
        "command": "dendron.exportPodv2",
        "args": "dendron.projects"
    },
```

## Steps

### Create a new project
1. Create a new project using the following hierarchy: `proj.{year}.{month}-{title}`
1. This will automatically apply the [[Project|dendron://private/templates.project]] template 
1. When ready, upload the project by running export pod with the `dendron.projects` preset
1. Also add the project to [[2022|dendron://private/proj.2022]] (NOTE: we'll update the link here on a yearly basis)


### Update a project
1. Inside a project, run export pod with the project preset to update a project
1. You can view your updated project in [[airtable|dendron://private/s.airtable.ref.projects#^2T71PdEpJFDe]]

### Add a task inside a project
1. Add a link to the tag inside the given project
    - NOTE: the task itself must have an airtable record id (aka already be uploaded to airtable)
1. Export the project

## Tips
- use [[Project Detail Dashboard|dendron://private/s.airtable.ref.base.tasks.interface.project-detail]] to see details of any particular project

## Examples

An example project: [[Setup Dendrologist Program|dendron://private/proj.2022.01-dendrologist]]
