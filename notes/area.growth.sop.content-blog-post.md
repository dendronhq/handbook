---
id: 03yxrn5tz5hhe1v0rhdzoch
title: Content Blog Post
desc: ''
updated: 1651529312180
created: 1650322474291
---

## Summary
Add a new blog post

## Prerequisites

## Steps
### Prepare the branch
1. Open up the terminal to the `dendron-blog` vault 
  - `> Terminal: Create New Integrated Terminal`
  - Select `Dendron.Blog`
1. Checkout a new branch 
  ```
  git checkout -b feature/{article-title}
  ```

### Posting
1. Create a new blog note at `blog.{YEAR}.{date-separated-by-dash}-{title}` inside of [[Blog|dendron://dendron.blog/blog]]
    - NOTE: the auto-generated title will include the date in the note title, be sure to remove it 
1. Apply [[Blog Post Template|dendron://dendron.blog/blog.temp.post]]
    - fill out relevant frontmatter
    - `date`: check the [[Publication Windows|dendron://dendron.handbook/area.growth.sop.content-blog-post#publication-windows]] and set the date to the earliest available publication window
    - `excerpt`: an 250 character or less description of the article
    - `image`: url to an image for the article 
1. Add blog post 
1. Add a header image
  - see [[Image Sources|dendron://dendron.handbook/area.growth.sop.content-blog-post#image-sources]] for list of open source image providers
  - follow process [[Upload Images|dendron://private/area.common.sop.upload-images]]
1. Submit for PR
1. When PR is approved, merge 
1. When the blog goes out, set `publish: true` and push straight to master

### After Release
1. Make sure the blog post is announced during the weekly release
1. Cross post the blog post in other channels by following [[Blog posts and cross-posting|dendron://dendron.handbook/area.growth.sop.social-media#blog-posts-and-cross-posting]]

## Examples
- [[Growing Knowledge Bases from the Bottom Up|dendron://dendron.blog/blog.2022.2022-04-05-growing-knowledge-bases-from-the-bottom-up]]

## Reference

### Publication Windows
- Mon-Th 7AM-11AM PST

### Image Sources
- https://www.pexels.com/

## Checklist

## Templates

## Lookup
