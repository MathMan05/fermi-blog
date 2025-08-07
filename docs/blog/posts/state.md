---
date:
  created: 2025-08-25
pin: true
links:
  - Homepage: index.md
  - Fermi: https://Fermi.com
categories:
  - Fermi
tags:
  - fermi
authors:
  - mathium05
slug: state-of
---

# The State of Fermi

The current state of Fermi is currently complicated, I've not been working on it as much as I would like due to irl issues. But I do plan to start working on it more now with additional privacy and school starting back up in a week or two.

<!-- more -->

**Things that need to be done:**

*	A new icon maybe for fitting the name Fermi?
*	VCs
	*	Firefox Support
	*	Call buttons
	*	Translation support for the status
	*	Pop out window for video
	*	Allow chatting in the channel as well
*	Scroller support in Webkit
*	CSS polish
*	Mobile fixes
*	DMs rework
	*	Groups
	*	A better indicator of which DM you're in
	*	Rework of the friends list
	*	VC support for DMs
*	Profile work
	*	Full screen profiles
	*	Display permissions of Members in a guild
	*	A send message bar in the smaller version
*	Keyboard shortcuts
	*	Basically everything

While I know these things do need to be done, some of these tasks are a lot harder than they may seem, like Firefox VC support are rather hard, though also rather critical for moving forward. I do plan to implement all of these eventually, some may just take longer than others.

There's also goals of eventually having support for the [Polyphony protocol](https://github.com/polyphony-chat), though this will be further into the future due to the slower pace of the project and the lack of gateway in the current state of the projects. Although once working the main server implementation should just work out of the box with Fermi due to their plans to have support for the Spacebar API.

## The State of Spacebar
While I do rather like Spacebar, there are some issues with the server and how it implements some things, it sometimes sends incomplete objects, or incorrectly formatted objects creating client issues. And sometimes it also forgets to deliver events which causes states not to be updated, I might do some more work on the Spacebar server, though I'm not a backend dev.

Working on Spacebar itself is one of the best ways to help me with Fermi due to my lack of backend dev skills, while I can do it, I am not fast at it.

## The State of the Main Instance
This is another issue that Spacebar faces, a whole chicken and egg problem, the main instance lacks users, so people don't want to join due to the lack of users. Though this issue is also made worse due to other issues, like incomplete clients, which includes Fermi, though I hope to help this issue with Fermi and updates to Fermi.

The main instance also doesn't have VCs enabled, which is too bad due to the demand for them, and the fact they're implemented in the backend, though it's also been having some issues running on NixOS which the main instance uses.
