---

links:
  - Homepage: index.md
  - Fermi: https://fermi.chat
  - Stoat/Revolt: https://github.com/stoatchat
authors:
  - mathium05
description: What's the deal with Revolt/Stoat? Is it a good discord alternative?
---
# What's the deal with Revolt/Stoat?
There is a lot to say about Revolt/Stoat. So let us start out with some of the positive things about it before talking about the rest.

Good things about Revolt/Stoat:

- Bridge bot support is excellent
	* It's pretty good with the ability to set per message pfps/usernames allowing for one bot without webhook perms to be a rather effective bridge.
- Mostly FOSS
- The client is meant for discord like communication
- The Bot libraries are decent
- Decent discovery
- Rust (if that's your thing)

I'm sure there's much more that I'm just not thinking about right now, but this is a list of some of the good things.

## Issues with Revolt/Stoat

### Non-FOSS components
Stoat/Revolt has many non-FOSS components, which does not inspire confidence from a FOSS project. There are two kinds of non-FOSS components that Stoat/Revolt has.

Firstly and way less egregiously are the source first components found at the [GitLab](https://git.is.horse/revolt) including the Discovery Feature, Authenticator Shield and the old Admin Panel (Which has since been remade with the aGPLv3 license [here](https://github.com/stoatchat/service-admin-panel), though we'll talk about this later). These projects licenses are based on the FUTO license, which say wether its good or bad, but it's not FOSS.

The Second issue is the new admin panel, which is under aGPLv3 with proprietary components, which is not allowed under the aGPLv3. They've known about this for at least half a year at time of writing, with a newly opened pull request [here](https://github.com/stoatchat/service-admin-panel/issues/5) attached to the repo. While I suspect they're not currently breaking any laws as is, (it's just the main team right now with no outside contributes at least it looks that way), it is not inspiring to see a project that calls itself FOSS to do these kinds of things.

### The AI Policy
[It does seem they're going to allow AI contributions](https://github.com/orgs/stoatchat/discussions/1022) though we've yet to really see the full scope of this, any many of the maintainers are pro-AI. We'll have to see how this evolves with time.

### The Great Rename
So, you might notice how there's been two names I've been calling them this whole time. Revolt and Stoat, that's due to a name change they underwent somewhat recently, Revolt -> Stoat. There's nothing wrong with doing a name change, the real issue is how it was done. The community was not aware of the name change before it was thrusted onto to them along with all of the client links redirecting to the new clients with a new interface making it a rather rough transition. Many people thought it was some sort of hack on Revolt and did not login to the new client for at least a few days to let the dust settle. 

They afterwards told users they both were planning to do this for a while and that they had recently gotten a cease and desist letter from some unknown company. (still unknown to this day of me writing this) The new client that they had pushed onto everyone was lacking compared to the old one, missing translation strings in spots and with temp link that were pointing to bogus websites. 

And still now many issues with the name transition persist. With parts of the client still saying Revolt instead of the new name, or URLs linking to the old project instead of the new one. 

## The More Minor Issues

### Hosting Requirements
It's just not really meant to be self hosted. [While they do let you and have instructions on it](https://github.com/stoatchat/self-hosted), the clients are just not made for this. You can't enter an instance URL to join an instance, so you'll have to distribute all of the clients yourself, including the mobile ones.

I've also been told that Revolt/Stoat is a bit of a RAM hog for whatever reason, making it harder to self host, though one can just host it despite that, so not a real issue, just a nitpick.

### Client/Server bugs
It's not exactly where many of the bugs lie, but stuff like read states is just broken on it. Like sending a message doesn't mark a channel as read, and sometimes being at the bottom of the channel doesn't do it either, often you have to leave and come back to the channel before the read state finally clears. On the new client you can't currently report people, due to part of the menu being off screen, while not directly their fault, they haven't done anything to fix this issue yet, just leaving the menu off screen for those who wish to report messages.

### Hard to Find Source Code
You might think that all of the source is under the github, and you'd be wrong. Some of the source is is proprietary repos, some of it is in the github some of it is in the [gitlab](https://git.is.horse/revolt/) that they don't link anywhere that'd kinda hard to find. And some lives [here](https://git.stoatinternal.com) though you can't access it. (it's not really clear what's here, when I asked about the gitlab I was also linked there)
