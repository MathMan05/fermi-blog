---

links:
  - Homepage: index.md
  - Fermi: https://fermi.chat
  - Spacebar: https://spacebar.chat
authors:
  - mathium05
description: Spacebar, a story of mismanagement
---
# Spacebar, a Story of Mismanagement
??? info
        Please note, this is going to be opinionated, though all of the facts will be true.

## The Beginning
Spacebar used to be an option I promoted, but the reality is that it’s been mismanaged into oblivion. This isn’t new or recent though; it’s always been mismanaged. For a while I hoped it would get better, and that my role within Spacebar would allow me to help fix it. I was wrong. It was not going to get better, and now a recent event likely set the project at least an entire year or two back.

In my time of contributing to Spacebar I had seen the many levels of mismanagement. For starters, there were people who were by all extents and purposes no longer involved with the project who still had admin power over the project, an [Open Collective](https://opencollective.com/spacebar) ran by someone who hasn't been involved in the project in a long time, a [dockerhub](https://hub.docker.com/u/spacebarchat) that had not been updated, and people constantly committing to main which means that code was added without any testing or review.

Some of the Spacebar team did treat me decently. Emma/Rory (one person, different usernames), had treated me with some respect and had tried to promote me within the Spacebar organization for a while, though had failed. I had done quite a bit of work on Spacebar, cleaning up the codebase and contributing many features and fixing bot support. I had even added features requested by the Spacebar team to help debug and improve Spacebar. However, even with all of that the respect and treatment from Spacebar had not been great.

I was never treated particularly well, with the creator of the React client talking down about my client. He would call it a simple client made in JavaScript and HTML before I switched to TypeScript, and while I did not take any offense to this at the time, it was just a small part of a larger pattern. He expected me to promote his client along side mine to all of the new users. After my client became the defacto official client, it was not expected of other clients to promote mine, not that I wanted that. 

There was another person who was admin in the discord guild that would come in to promote her project and say that Spacebar was not for serious use, disparaging it. Nothing was ever done by Spacebar as she was an admin within Spacebar despite not actually being involved in the project. There were many with power within the Discord, Spacebar, Github, and similar spaces despite not actually being with the project anymore, and Spacebar refused to fix this.

The codebase was also not doing too great. The TypeScript parts being less than good in sections, were doing things in technically correct ways that should not be done none the less. Things like modifying object prototypes which broke dependencies, something that is considered a really bad practice in TypeScript. I removed this pre-fork, which caused one of the maintainers to take it as a slight against them. Some other examples: Not using the type checker the API used for the gateway, which made the gateway strange and harder to maintain. Code quality issues in general, partly due to people committing to main, and partly due to low code standards letting less than ideal code get in. Even some of my early code should not have been allowed in, because the way I originally handled mentions was not good. Models in schemas leaked information. And a total lack of testing which meant that features broke often.

## The incident

While all of that was less than great, it was not enough to cause me to feel the need to jump ship quite yet. 

On March 29, 2026 I was banned from the Spacebar Discord for arguing against AI use in projects. They now claim it was for other reasons, but this was the actual incident. Did someone who was active within the project ban me? No. It was someone who had admin despite not being active within development for more than two years, and not even being on the Spacebar platform itself. The existing moderation had minimal oversight and little concern for what the rules might be. It had a two yes approval system, and even this was not followed (another mod showed me the screenshots). Not only did they ban me from the Discord, but the Spacebar guild as well and other spaces unrelated to the ban. I was not informed of the ban before it happened, and the only reason I had gotten that information is due to me asking for it.

The community wanted answers. Instead of providing them, they decided to troll the community rather than actually address people's concerns. When they did eventually put out an announcement, it was so vague that many people were confused by what it meant or came away thinking that I was pro-AI, despite being well known for strongly disliking AI. They also claimed I was hard to work with as a contributing reason for my ban, whilst being told in DMs that I was free to continue working on Spacebar after this ban by the Spacebar team. After all of the backlash from the community this individual left the project with an accompanying announcement about it, although not really. She kept her admin roles within the Discord for unknown reasons and there was nothing anyone within the project could do as the owner account was lost to time. This all occurred over roughly 3-4 days.

## The Aftermath

One might think that this would be enough to get the project to rethink and fix itself, though that is not what happened. Instead, the project just froze. I waited for 2 weeks after the initial announcement for for anything to happen, even something as simple as a statement or DM from a team member within Spacebar saying that this whole situation was bad would've been enough. Those 2 weeks came and went and nothing was said, the most I got were many statements saying that Emma (it/its) had not agreed to the ban, being carefully worded to not say its actual opinion on the ban. I was told that I should wait 1-6 months before doing anything as that's how long it'd take for it to decide whether or not the ban was justified.

There were many people who insisted I should've waited longer, or should've worked for Spacebar despite being banned. I was not going to wait that long for an apology, let alone for this to start to be resolved. Considering all the other issues leading up to this incident, the decision was made to fork Spacebar to continue it under better management if nothing happened within two weeks. Even though I was kicked out of Spacebar by Spacebar there were many people who were upset at me for creating a fork, even though I tried to wait for any kind of solution first. There was roughly a period of a month where if things did start to seriously improve I would've considered going back, but they didn't. Now the organizational issues are arguably worse. While the people who should not have had power before were mostly gone, there was no one to take their place. The maintainer was unable to lead the project, and those who were left were not suited for leading. One of the current admins on Spacebar in the aftermath of the ban was known for trolling and making the conversation harder than it should've been. The same individual later came into the Harmony community on an alt to attempt to stir controversy, followed by their main account, and then denied that the alt was theirs despite the profiles and usernames being directly linked to each other and the chat repeatedly calling them out on it.

At this point Spacebar has no real leadership, and their structure has been damaged further due to not being willing or able to take steps to actually fix the project. You either have to to use a client that's a fork of Fermi by someone who is well known for being pro-AI and who tried to change the AI policy within their fork to align with their views on AI (this detail was later git purged and lost to time after the project was removed from GitHub) or are forced to use one of the incomplete clients, many of which are proprietary.

I was a part of the Spacebar team to an extent, though I was always kept out of being officially part of the team. Despite being the one who created Fermi, frequently reviewed PRs and many of the changes that went through without review otherwise; I was not respected, involved in any decision making for the project, nor was I allowed in further than being a contributor to the project. Spacebar wanted me to have many of the responsibilities of being in the project but did not actually want to give me any position within it. I only have a few vague suspicions, but beyond that I really have no idea why I faced this treatment because no one ever communicated with me about it. I honestly do not know why they treated me this way.

I also did end up forking Spacebar into Harmony two weeks after ban. Harmony is the continuation of Spacebar without all of the structural problems and with much higher standards for code quality and review. This continuation will seek to have better compatibility with bot libraries and seek to pose itself as a more serious alternative to discord with the maturing of both Fermi and Harmony's codebases.

### Addendum (6/26/2026):
The AI fork of Fermi has now made the source code non-public, its been that way for a few days, but I was waiting for it to unscrew up in this way. This is both further disappointing and expected. From what I've heard from others they plan to keep it as a soft fork so it seems like it'll be Fermi but with a different name.
