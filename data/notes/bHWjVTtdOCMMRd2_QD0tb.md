
Dendron has a lot of moving parts and can feel a bit daunting to start working on a feature or a fix if the particular area of Dendron is new to you.
Figuring out how everything works would be nice in an ideal world but it's often better to seek help from other team members who are familiar with the area.

Below are some things to try if you are stuck.

## Things to try before asking

Lookup is a very important concept in Dendron itself and also as our company value as we describe [[here|handbook.company.values#lookup]].
Because of this, it is most likely that an existing feature would have it's own documentation written already.

1. Identify what part of the codebase is relevant to the feature you are working on.
1. Try a quick `lookup` on the feature in this workspace and see if any note can give you the information you need.
    - Specific features of Dendron will usually be described in `dendron.topic.*`
    - Project related notes will be under `pro.*`
1. Adding breakpoints and running the extension to just look into what is going on under the hood is also a good way to get a rough idea of what should be done.
    - See [[Debugging Tests|dev.process.qa.debug]] for more information on how to do this.
1. If this is not enough, consider asking for help (see below).

## Asking for help

If troubleshooting yourself was not sufficient, you can seek help from other people in various places.

1. Try asking specific questions in the `#dev` channel or `#dendron-team` channel of our Discord server.
    - `#dev` is a public channel so your questions could get more exposure to people.
    - An added bonus to preferring discussions in the `#dev` channel over private channels or DM is that other people (especially community members) can see this and use it as a reference if they decided to contribute in the future.

1. If the issue isn't resolved yet, consider scheduling a pairing session with Kevin or anyone who has had prior experience working on the subject matter.
    - Team members will have set up their calendars according to [[this guideline|templates.people.onboarding#calendar]] 
    - They will usually have available schedules listed in their user hierarchy (`user.{name}`). Otherwise, ping them or DM to find the best time.
        - Kevin's calendar can be found [[here|dendron://private/user.kevin.ref.cal]], for example.

1. If you have already started writing code, another good thing to do is to open a draft pull request on Github and pushing the progress you have made so far.
    - This way other people can comment directly on your changes, and possibly work out the kinks asynchronously without you having to schedule a real time pairing session.

## After getting help

- To transform the troubleshooting efforts you have gone through into a permanent piece of knowledge, consider improving the existing documentation or add a new entry to our documentation with your findings.
- This will make a positive feedback loop of improved documentations and easier troubleshooting for yourself and others in the future.
