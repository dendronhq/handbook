---
id: yTP0DBIpfDyRAc9EMPUKJ
title: Issues in Airtable
desc: ''
updated: 1641595477470
created: 1638884656443
---

## Setup

> Note: This workflow is in flux and is subject to change

This example demonstrates how to setup an Export Pod V2 to Airtable for Dendron Tasks

### Create a new Airtable Connection

![[dendron://incubator/s.airtable.sop.connect-to-airtable#connect-airtable-using-dendron-export-pod,1:#*]]

### Run the Pod to Export a Task to Airtable

1. Open a task note that you want to export to airtable.  An example task note is [[task.pod.podsv2-support-export-hierarchy]]
1. Run `Dendron: Export Pod V2` while your task note is in focus.
1. Select `dendron.tasks`
1. Check the [task view here](https://airtable.com/appKOgvtfSzZyj1YM/tblLjBKhYtXnZ2t1w/viwzfUhwxGiomaGjt?blocks=hide) in our Airtable here to see if the task was successfully added.
1. If it's not added, then check out common errors below

### Troubleshooting

- You get an error like the following:
    ```
    "Error while running Airtable Export Pod: {\"error\":\"INVALID_MULTIPLE_CHOICE_OPTIONS\",\"message\":\"Insufficient permissions to create new select option \\\"\\\"NON-REPRO\\\"\\\"\",\"statusCode\":422}"
    ```

    Some fields in Airtable are like enums - if you try to upload a value that's not in the enum set, then you'll get this error. Scope, Size, and Status are enum fields. Scope must match a value in [[tags.scope]].  When in doubt, check what values are allowed in airtable.
