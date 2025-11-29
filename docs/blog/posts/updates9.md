---
date:
  created: 2025-11-28
pin: true
links:
  - Homepage: index.md
  - Fermi: https://fermi.chat
categories:
  - Fermi
tags:
  - fermi
authors:
  - mathium05
slug: updates
comments: true
description: This week in Fermi there are a barrage of improvements, including Passkey 2FA support, Timeouts, Slowmode and @here. Along with various work on Spacebar itself with bug fixes and improvements.
---

# Passkeys, Timeouts, Slowmode, and @here, This Week in Fermi
This week in Fermi there are a barrage of improvements, including Passkey 2FA support, Timeouts, Slowmode and @here. Along with various work on Spacebar itself with bug fixes and improvements.

<!-- more -->


## this weeks updates

### Passkey 2FA Support
Fermi now supports passkeys as a 2FA method! This means that you can use the various sources of passkeys, which include but are not limited to, phones, windows hello, the physical passkey devices and NFC passkeys. This should help secure your accounts and ensure the safety of your spacebar accounts with better ease of use. (To take advantage of this you must also have time based codes enabled)

### Timeout/Slowmode Support
This week in Spacebar I've implemented Timeout and Slowmode support into Fermi, so now you can now moderate users with a Timeout, or enforce a Slowmode, which should help with guild moderation! I also implemented Slowmode into the Spacebar server itself, with [Emma](https://github.com/TheArcaneBrony) implementing Timeouts!

### @here
You can now ping @here inside of Fermi along with seeing @here pings render correctly! They ping just the people who are online, and just like every other type of ping, they should persist correctly across sessions!

### Minor improvements
* Login shows on the app page instead of force directing you to the login page
* You can now delete applications from the dev portal [Implements](https://github.com/MathMan05/Fermi/issues/176)
* Nonce is now used to prevent duping of messages
* Emoji packer is now in TS [Implements](https://github.com/MathMan05/Fermi/issues/170)
* You can now add people to DMs [Implements](https://github.com/MathMan05/Fermi/issues/174)
* Groups member lists now update when a person is added/removed from the group
* Usernames of blocked people should now resolve to "Blocked User".

### Bug fixes
* Fix DM unreads bug
* Messages no longer fail to send sometimes
* Favorites Object failed to clone old in some cases 
	- [Fixes](https://github.com/MathMan05/Fermi/issues/178)
* Corrected Gif Favorite types after spacebar changes
	-	Truly no clue how it happened :P
* Fix bug where you couldn't clear read state on DMs sometimes
* DMs unreads didn't work properly
	- [Fixes](https://github.com/MathMan05/Fermi/issues/179)
* Copy User ID on DMs now only shows for dms instead of showing for DMs and groups with just one person.
* CREATE_CHANNEL that's fired for existing channel will no longer create dupe channels

### Mitigations
* none this week

### Discovered Spacebar Bugs
* Deleting apps doesn't work.
	- Was also fixed

### Spacebar fixes
* [Interaction callbacks now support mentions, link embeds, and epheral messages work normally](https://github.com/spacebarchat/server/pull/1396)
	- [Fixes](https://github.com/spacebarchat/server/issues/1369)
* [Fix deleting apps](https://github.com/spacebarchat/server/pull/1404)
* [Centralize permission checking](https://github.com/spacebarchat/server/pull/1405)
* [Implement Slowmode](https://github.com/spacebarchat/server/pull/1406)
* [Removed an unneeded log](https://github.com/spacebarchat/server/pull/1409)

### For Those Who Want More Details
I've gone through and removed some fake polyfills from the spacebar codebase, which should make the code much more maintainable, and fixes some breakages with the SDP parser that the experimental WebRTC implementation needs to work correctly. I've also gone through and centralized permission checking a bit, making it easier to overhaul how permissions are calculated a bit, which made for Timeout/Quartine support in the server itself easier to create for the other maintainers. 

For those who are wondering about WebRTC progress, while I myself haven't done anything other than removing the polyfills that blocked the codebase from functioning correctly, it seems that some progress has been made, and the person who's making WebRTC work now has permissions to publish the WebRTC code by themselves, which should help with updates. I've also heard that recent updates to the WebRTC codebase should make it run on the linux distribution that the main public instance uses, which *should* hopefully mean that WebRTC is closer to being ready. Please try to not get your hopes up, while it is closer to being ready than ever before, it very well could take more time for it to work, or to be a more polished user experience. Once it is working I will have to go through and do some more polish in Fermi to ensure that users have the best experience with voice chats as they possibly can! (though it should just work once it's enabled, though I'd like to finish up on some things)

While not implemented in Fermi, the server also now has the ability to send the recent ping endpoint, which could be implemented into Fermi if there is interest in that. But this should be noted as other clients might use this endpoint. There's also been steps to prevent situations where the access token key might get lost, and similar steps have also been taken to stop them from being constantly read off of the disk and cache it in memory. (thanks Emma again for all of these nice patches)

Admin API now requires the OPERATOR RIGHT to access, and it did not before, though please note that this was not an issue before, as it was an optional component, and was not enabled by default, though now it should be more secure to expose it. (Thanks to Emma for fixing this)


### The Best Way of Reporting Bugs/Feature Requests
If you want to be credited and have better chances of your ideas coming to life please [submit an issue on github](https://github.com/MathMan05/Fermi/issues)! This makes things easier for me as everything is in one place, and you can be credited in the blog posts as well via a link to the issue you have created!

If you guys have anything you'd like to see feel free to [open an issue](https://github.com/MathMan05/Fermi/issues/new) or say your ideas in the [Fermi Spacebar guild](https://fermi.chat/invite/USgYJo?instance=https%3A%2F%2Fspacebar.chat) or even the [Spacebar Discord Server](https://discord.gg/JDjMXTGeY9)
