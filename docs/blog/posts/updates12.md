---
date:
  created: 2025-12-22
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
description: This week in Fermi I've implemented Friend nicknames, session management and much much more!
---
# Session Management, Friend nicknames and bug fixes!
This week in Fermi I've implemented Friend nicknames, session management and much much more!
<!-- more -->
(sorry for being a little late y'all)

## this weeks updates

### Session Management
You can now logout devices that you don't want in your account! (or some pesky hackers!) You'll also be able to see a lot of information about all of the devices, including aproximate location and IP address

### Friend (Or Enemy) Nicknames 
You can now set nicknames of people you have a relationship with! (which means friends, enemies, people who've sent you a friend request or vice versa)

### Minor improvements
* Fermi no longer uses express.js
* CDN is better cached
* Connections are now typed
* Added Dev setting to disable gateway compression
* Added @ to the escapable markdown chars
* Usernames update live in Femri in most places
* Manage nicknames now works as expected
	- [Implements](https://github.com/MathMan05/Fermi/issues/149)
* Not-rich embeds are now standard widths again
* Switching setting pages no longer animates
	- This was ugly, and has been removed due to that
* Settings doesn't repeat itself for form errors
* Guild names not matching shows up as a translated form error now in the delete menu
* Unknown role is now translated
* Updated GIF/Sticker icons to look better
* Channels share Map objects to help with load


### Bug fixes
* Webkit now has another polyfill allowing Webkit to work correctly now
* Login screen now returns errors
* Hyper logging is no more
* Potential redir exploits are fixed
* Gateway reconnection attempts now work more betterer
* Member list works correctly in DMs again
* Password fields in settings now are password

### Mitigations

### Discovered Spacebar Bugs

### Spacebar fixes
* [Fixed minor bug that broke bot invites](https://github.com/spacebarchat/server/pull/1438)
* [Relation Nicknames](https://github.com/spacebarchat/server/pull/1442)
* [Fixed Bot DM bug](https://github.com/spacebarchat/server/pull/1448)
	- Thank to [Jersey](https://williamhorning.dev/) for pointing this out on the spacebar discord server

### The Best Way of Reporting Bugs/Feature Requests
If you want to be credited and have better chances of your ideas coming to life please [submit an issue on github](https://github.com/MathMan05/Fermi/issues)! This makes things easier for me as everything is in one place, and you can be credited in the blog posts as well via a link to the issue you have created!

If you guys have anything you'd like to see feel free to [open an issue](https://github.com/MathMan05/Fermi/issues/new) or say your ideas in the [Fermi Spacebar guild](https://fermi.chat/invite/USgYJo?instance=https%3A%2F%2Fspacebar.chat) or even the [Spacebar Discord Server](https://discord.gg/JDjMXTGeY9)
