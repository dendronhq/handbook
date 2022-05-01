---
id: q4q3ajj5lqbh596mw5ag6wf
title: Actions
desc: ''
updated: 1647011557625
created: 1645808599337
---

### Nightly
- action: https://github.com/dendronhq/dendron/actions/workflows/publish-extension-nightly.yml
- workflow file: https://github.com/dendronhq/dendron/actions/runs/1897318612/workflow

```yml
# See documentation on POSIX cron syntax here: https://docs.github.com/en/actions/reference/events-that-trigger-workflows#scheduled-events
# Scheduled to run every weekday at 12:00 AM PST, which is 7:00 AM UTC Tuesday-Saturday
on:
  workflow_dispatch:
  schedule:
    - cron: "0 7 * * 1-6"
```

### Create Release Image
- url: https://github.com/dendronhq/dendron/actions/workflows/create-release-image.yml
