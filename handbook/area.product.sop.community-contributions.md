---
id: fcd56ea9-a0e0-4d23-b32e-12d4e70c4f09
title: Community Contributions
desc: ''
updated: 1646957299201
created: 1618274414190
---

## Summary

This should be done whenever anyone submits a pull requests, updates the documentation or submits a bug request to Dendron

## Checklist

1. Add user to Community Updates of the weekly journal
    - see example [[Community|dendron://private/weekly.journal.2022.03.15#community]]
    - eg: 
    ```markdown
    ## Community
    <!-- Recognize comunity contributions -->

    - [dagriefaa](https://github.com/dagriefaa)
      - #role.bugcatcher
      - [Favicon not rendering when assetPrefix is set](https://github.com/dendronhq/dendron/issues/2536)

    - [chmac](https://github.com/chmac)
      - [Lookup stops working properly after pressing tab](https://github.com/dendronhq/dendron/issues/2550)
    ```
2. If the user exists, you should be able to auto-complete
   - If the user doesn't exist, create them (make sure to create them in dendron-private vault)
   - Add as much metadata as possible
     - `[Firstname Lastname](link to github url) discord alias`
     - eg. `[[Dendron User|people.dendron-user]]`
3. Have a line explaining their contribution
4. If this is their first bug report/pull request/etc and they are on Discord, award them the appropriate badge 
   - make sure to note the accomplishment in dendron using a tag inside the `people.*` note
   - For a list of all roles and their meaning: [[Roles|dendron://dendron.dendron-site/community.discord.roles]]
     - eg. `#role.bugcatcher`
   - also add this to the entry

## Example

```
- [[people.dendron-user]]
  - #role.taxonomist
  - [fix typo](https://github.com/dendronhq/dendron/issues/617)
```

## Related

- [[Roles|dendron://dendron.dendron-site/community.discord.roles]]

