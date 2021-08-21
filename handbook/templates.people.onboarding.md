---
id: c6b422a5-204a-41dd-8e47-f0b736160790
title: Onboarding 
desc: ''
updated: 1629489032871
created: 1620248731246
---
## Welcome to Dendron!

We are so excited you’re here and look forward to setting you up for remote-first success as your journey begins. Copy this onboarding checklist to user.{alias}.onboarding in the private vault and work through the tasks over the course of your first 30 days. If any task doesn't make sense, please reach out to the team on discord. 

- **Note:** We're really appreciative of Gitlab pioneering the space of remote work and have included a lot of links to the Gitlab handbook. The wealth of information in this note can be overwhelming at times. It's okay to skim through resources, bookmark them and come back at a later time.

## Table of Contents

- Day 1: [Getting Started: Intro, Accounts and Paperwork](#day-1-getting-started-accounts-and-paperwork)
- Day 2: [Morning: Remote Working and our Values](#day-2-remote-working-and-our-values)
- Day 3: [Morning: Social](#day-3-social)
- Day 4: [Morning: Git](#day-4-git)
- [Job Specific Tasks](#job-specific-tasks)

## Introduction

This is your core onboarding issue and it is housed in Dendron in the interests of what is known as [dogfooding](https://about.gitlab.com/handbook/values/#dogfooding). It has been crafted with the [three dimensions of remote onboarding](https://about.gitlab.com/company/culture/all-remote/onboarding/) in mind, namely: Organizational Onboarding, Technical Onboarding and Social Onboarding.

All three of these are underpinned by the sentiments of [lifelong learning](https://handbook.dendron.so/notes/b89ba854-72fb-4ebc-a8a0-55960b89e9dc.html#lifelong-learning), while encouraging [asynchronous communication and workflows](https://about.gitlab.com/company/culture/all-remote/asynchronous/).

## Support and our Single Source of Truth

Since Dendron aspires to be a [handbook first](https://about.gitlab.com/company/culture/all-remote/handbook-first-documentation/) organization, the answer to question you may have particularly throughout your first thirty days should be documented and readily available in the [handbook](http://handbook.dendron.so). If you are unable to find the information you are looking for, please reach out on the #dendron-team channel in Discord and update the handbook once you find the answer.

## The First Thirty Days

This note consists of a series of tasks which should be completed sequentially over the course of the next thirty days structured as follows:

| Day        | Area of Focus                                |
| ---------- | -------------------------------------------- |
| **Day 01** | Intro, Accounts and Paperwork                |
| **Day 02** | Remote Work: Communication and Values        |
| **Day 03** | Organizational Structure and Social Elements |
| **Day 04** | Introduction to Dendron and using Github     |

Though you may be eager to jump right into your role we encourage you to set aside dedicated time every day for your first week to focus on these tasks as they are geared toward ensuring you are enabled to [thrive in an all-remote environment](https://about.gitlab.com/company/culture/all-remote/onboarding/#the-importance-of-onboarding).

## Continuous Improvement

In the interests of paying it forward and contributing to our core value of [Iteration](https://handbook.dendron.so/notes/b89ba854-72fb-4ebc-a8a0-55960b89e9dc.html#iteration) - we encourage you to suggest changes and updates to this note and the handbook, both of which can be done via Pull Request (PR).

Along with this you will complete onboarding on Day Thirty by being asked to fill out the [Onboarding Satisfaction Survey](https://airtable.com/shrcILcL6cm6lpCZt), which is an opportunity to share feedback on your general Onboarding Experience.

* * *

> Note: You'll see certain comments throughout this checklist to clarify what is applicable to you. The comment is valid till the next section/heading. They are:
>
> - `<!-- Full time -->` applies only to team members that are working on Dendron full time (includes full-time contractors + interns)
> - `<!-- Trial -->` applies to team members that are working on limited duration projects (2-4 weeks)
> - `<!-- Hourly -->` applies to team members paid by the hour.
> - If not specified, sections should be applicable to everyone.


## Day 1 - Getting Started: Accounts and Paperwork

#### Daily Journal Note

1. [ ] Start the daily journal note for today. You can read more about it [[here|schemas.user#dailyjournal]]

<!-- Hourly -->

1. [ ] Please include two additional frontmatter fields that track the hours you've worked. It should look something like this:

```
---
id: c6b422a5-204a-41dd-8e47-f0b736160790
title: Daily note
desc: ""
updated: 1622543447981
created: 1620248731246
hoursToday: 8
hoursMonth: 48
---
```

#### User Intro
- [ ] Create and add your own [[user readme|templates.user-readme]]. This may take some time to create so please feel free to iterate on it once you get some details in to your user.<name> hierarchy in Dendron.

#### Rpass

1. [ ] :red_circle: Install rpass. Dendron provides all team members with an account to rpass to help manage work credentials.

#### 2FA (Two-Factor Authentication)

2. [ ] Dendron requires you to enable 2FA (2-Step Verification, also known as two-factor authentication), because it adds an extra layer of security to your account. You sign in with something you know (your password) and something you have (a code you can copy from your Virtual Multi-Factor authentication Device, like [Authy](https://authy.com), FreeOTP, or Google Authenticator). Please make sure that time is set automatically on your device (ie. on Android: "Settings" > "Date & Time" > "Set automatically"). If you have problems with 2FA just let the team know! We can disable it for you to then set it up again. Reach out proactively if you're struggling - it's better than getting locked out and needing to wait for IT Ops to help you get back online.

3. [ ] :red_circle: Do the next 3 steps Today. Actually -- why not RIGHT NOW. This absolutely must be done within a week or you will be locked out and need to wait for an admin to get around to helping you get reconnected.
   1. [ ] :red_circle: Enable 2FA on your Dendron email account (Gmail/GSuite) (this should have been an option to do when you first received the invitation to the account).
   2. [ ] :red_circle: Enable [two-factor authentication](https://docs.github.com/en/github/authenticating-to-github/configuring-two-factor-authentication) on your Github account.

#### Rippling

**_This section is super important to ensure payroll + operations support. Please complete these items on your first day if possible._**

1. [ ] Rippling is our HRIS (Human Resource Information System) for all team members. We have self-service enabled so that at any time you can access your account to see your employment information and documentation. As part of onboarding, please make sure to update everything that is applicable to you.
   1. [ ] Access the Rippling [Dashboard](https://app.rippling.com) and make sure you complete any outstanding tasks assigned to you.
   2. [ ] For contractors being paid by the hour, it may be useful to save an invoice template for future use. An invoice template can be found in Google Docs by searching `Invoice Template` or [here](https://docs.google.com/spreadsheets/d/1faslC4H_NSLsk8jd8xUuwgAjqhkdSlaI0D1WINA1y9Y/edit#gid=0).
2. [ ] Don't forget to comply with the contract you signed, and make sure you understand [Intellectual Property](https://about.gitlab.com/handbook/people-group/code-of-conduct/#intellectual-property-and-protecting-ip).

#### Discord

1. [ ] Register on Discord by following this [invitation link](https://discord.gg/xrKTUStHNZ). Read the next suggestions on how to choose a username first.
2. [ ] You can use your personal discord OR choose to create a new username using your Dendron email. It's generally helpful to choose a username to be the same as your Github handle, for consistency and ease of use.
   1. [ ] At Dendron [Transparency](https://handbook.dendron.so/notes/b89ba854-72fb-4ebc-a8a0-55960b89e9dc.html#transparencyy) is a value and we prefer to use Public channels in Discord. Continue to use public channels wherever possible (`#dev`), especially if it is a work related discussion (you may be surprised by the feedback you get from the community).
   1. Make sure your Discord profile has a **photo** - it makes it easier for other team members to remember you!
1. [ ] If you're new to Discord, a short primer can be found at [a Beginner's guide to Discord](https://support.discord.com/hc/en-us/articles/360045138571-Beginner-s-Guide-to-Discord).
1. [ ] We also encourage you to message with community members in #questions and #feedback.
   - There are lots of other more informal channels (like #note-taking) where interesting stuff happens so check those out as well.
1. [ ] Make sure you have access to the #dendron-team channel and post an intro.
   1. This can be the [[About me|templates.user-readme#about-me]] that you used for your README
   1. We love to hear more, such as where you were before, family/pets, and hobbies.
   1. We also enjoy pictures if you're willing to share. Consider giving your new team members a glimpse into your world (scroll through previous messages in the channel for inspiration).

#### Other
- [ ] Accept calendar invite to the Dendron Company Calendar

#### Workspace Setup

Go to [[Job-specific tasks|templates.people.onboarding#job-specific-tasks]] and complete setting up your workspace. 
* * *

## Day 2 - Remote Working and our Values


### Remote Work

<!--Trial/Part-time optional-->

The first month at a remote company can be hard. **There is as much to unlearn as there is to learn**. Gitlab's a pioneer in this regard and have put together a great set of tips and tricks that will help. You can view their entire course listed below.

- [ ]  If you're new to working in a 100% remote environment, read over the [Guide for starting a new remote role](https://about.gitlab.com/company/culture/all-remote/getting-started/). You'll find other tips for operating (and thriving!) in an all-remote setting within the [All-Remote section of the Gitlab handbook](https://about.gitlab.com/company/culture/all-remote/). Take some inspiration from the folks at Gitlab on how they structure their remote working day, read this helpful blog post [A day in the life of remote worker](https://about.gitlab.com/blog/2019/06/18/day-in-the-life-remote-worker/)
- [ ]  Learn more about the `#allremote` onboarding process and additional [best practices](https://about.gitlab.com/company/culture/all-remote/learning-and-development/#how-do-you-onboard-new-team-members).
   - [Adopting a Self-Service and Self-Learning Mentality Knowledge Assessment](https://about.gitlab.com/company/culture/all-remote/self-service/#introduction)
     (Day 1)
   - [Informal Communication in an All-Remote Environment Knowledge Assessment](https://about.gitlab.com/company/culture/all-remote/informal-communication)
   - [Embrace Asynchronous Communication](https://about.gitlab.com/company/culture/all-remote/asynchronous)
   - [All-Remote Meetings](https://about.gitlab.com/company/culture/all-remote/meetings)
   - [Communicating Effectively and Responsibly Through Text](https://about.gitlab.com/company/culture/all-remote/meetings/#how-do-you-do-all-remote-meetings-right)
   - [Building and Reinforcing a Sustainable Culture Knowledge Assessment](https://about.gitlab.com/company/culture/all-remote/building-culture/#gitlab-knowledge-assessment-building-and-reinforcing-a-sustainable-culture)
   - [Combating Burnout, Isolation, and Anxiety in the Remote Workplace](https://about.gitlab.com/company/culture/all-remote/mental-health)
   - [The Non-Linear Workday](https://about.gitlab.com/company/culture/all-remote/non-linear-workday)

### Values

1. [ ] Dendron values are a living document. Familiarize yourself with our [[values|handbook.company.values]]
2. [ ] We are driven by our mission -  to help **people** organize and make sense of any amount of information.  Read our [[mission statement|handbook.company.mission]]

### Calendar

#### Set Up

- [ ] Set your Google Calendar [default event duration](https://calendar.google.com/calendar/r/settings) to use `speedy meetings`
- [ ] Set up [Calendly](https://about.gitlab.com/handbook/tools-and-tips/other-apps/#sts=Calendly). Calendly is a calendar tool that allows individuals to select open meeting slots in order to speak with others outside of Dendron. For Dendron team members, feel free to schedule directly through Google calendar. When you are setting up Calendly, there is no specific Dendron account. With the free version you will only be allowed one meeting time, but if you need to upgrade to a Pro account, you can do so and expense it.
- [ ] Add the Zoom integration by going to the `Integrations` section at the top of the page. Find Zoom in the list of integrations and click it. It will then ask you to link your Calendly and Zoom accounts together. Do so.
- [ ] Now make Zoom the default event location by editing each 'Event type' in Calendly (By default, there should be a `15 Minute Meeting`, `30 Minute Meeting` and `60 Minute Meeting` event types) by clicking the gear icon associated with each event type then going to `Edit`. Click on `What event is this?` and under `Location` choose Zoom. Click on `Save and Close`, and do this for each remaining event type.
- [ ] [Set your working hours & availability](https://support.google.com/calendar/answer/7638168?hl=en) in your Google Calendar.

#### Events

On your calendar, you will have a invites to the below meetings, Please note: These meetings may not fall during your first week.

1. Weekly planning sync. This is where the team reviews goals accomplished during the last week and picks up on what should be done this week to be successful.


## Day 3 - Social


### Social media + Expenses

- [ ] Connect with or follow Dendron's social media sites:
      [LinkedIn](https://www.linkedin.com/company/dendron-so/),
      [Twitter](https://twitter.com/dendronhq),
      [YouTube](https://www.youtube.com/channel/UC8GQLj4KZhN8WcJPiKXtcRQ).
- [ ] Familiarize yourself with our [[expense report process|dendron.sop.expensing]] and bookmark the [link](https://airtable.com/shrtJd0sitnY6Bfre) to expensing stuff.


* * *

## Day 4 - Dendron + Github

For those new to Github and Dendron, it's important to get familiar with the below and [bookmark these links](https://about.gitlab.com/company/culture/all-remote/self-service/)

### General Breakdown

1. [ ] Read how devs can [contribute](https://wiki.dendron.so/notes/81da87be-2d4e-47b5-a1d6-c0d647e1ab00.html) to Dendron.
2. [ ] Read [this page](https://wiki.dendron.so/notes/3489b652-cd0e-4ac8-a734-08094dc043eb.html) and all child pages for an overview of the Dendron Development Process

#### Issues and Issue Trackers

- [ ] Learn how to use [Github Issues](https://github.com/dendronhq/dendron/issues). We use Github Issues to raise awareness, discuss, and propose solutions for various issues related to any aspect of our business. The most common issues are created in the following projects:
   - [Dendron](https://github.com/dendronhq/dendron/issues) - Issues related to
     our main tool.
   - [Dendron Site](https://github.com/dendronhq/dendron-site/issues) - Issues related to documentation.
- [ ] Make an improvement to the [handbook](https://github.com/dendronhq/handbook). Being new, you may be unsure if your idea for a change is good or not, and that's OK! Your pull request starts the discussion, so don't be afraid to offer your perspective as a new team member.
   - [ ] Handbook: Assign the pull request (PR) to your onboarding buddy (if they have merge rights; if not, assign to your manager).

### Survey
- [ ] Set a reminder for 14 days past your start date to complete the [Onboarding Survey](https://airtable.com/shrcILcL6cm6lpCZt). We're actively trying to improve this process so please be proactive in reporting issues (or fixing them).

## Job-specific tasks

* [[Engineering|handbook.people.onboarding.engineering]]
* [[Content|handbook.people.onboarding.content]]


## [Lookup](https://handbook.dendron.so/notes/b89ba854-72fb-4ebc-a8a0-55960b89e9dc.html#lookup)

This section is both inspired by and borrows heavily from the following projects:

- [Gitlab](https://about.gitlab.com/handbook/) ([license](https://gitlab.com/gitlab-org/dco/blob/master/README.md))
