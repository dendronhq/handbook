---
id: qkgzoi28u5ar3w69rfajul1
title: Discord Thread Cutoff Reminder
desc: ''
updated: 1660877226583
created: 1660706472791
---

> Make sure to change the values `NEXT_WEEK` and `THIS_WEEK` in the template.

```markdown
@Dendron Team

Another reminder that the release branch has been snapped on Thursday 7PM (UTC), and all commits merged to master after that point is not in the release branch.

Make sure when you are adding items to `Ready to Ship`, that you are adding them to [[weekly.journal.{NEXT_WEEK}]]

If you have a commit that didn't make the cut-off but has to go out with this week's release, please leave a message here so that it could be properly cherry-picked and smoke tested in a timely manner.

Otherwise, I will be starting the process of preparing the early seed release based on the current state of the branch and the items listed in [[Ready to Ship|weekly.journal.{THIS_WEEK}#ready-to-ship]]
```