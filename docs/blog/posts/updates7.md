---
date:
  created: 2025-11-14
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
description: The last two weeks in Fermi I've added a reworked audio system which should fix many of the issues the old one had, a new menu for the dev settings, and the ability to add users to the channels permissions page!
---

# Audio Rework, Dev settings, Users in the Permissions menu for channels and more!
The last two weeks in Fermi I've added a reworked audio system which should fix many of the issues the old one had, a new menu for the dev settings, and the ability to add users to the channels permissions page!

<!-- more -->


## this weeks updates

### Audio System rework
The whole notification audio system of Fermi has now been reworked to be a lot better, this should hopefully get rid of the many snags of the old implementation.
([fixes](https://github.com/MathMan05/Fermi/issues/126))

### Developer Settings Menu  
I've added a special menu to hide away special developer settings instead of mixing it in with the rest of the settings. This should help with general orginization and some logging issues. 

### Users in the Channel Permissions Settings
You can now add individual users to the permissions settings so you can alter their individual permissions on a per channel basis.

### CSS un-nesting
This should allow for browsers that don't support CSS nesting to run Fermi, as Fermi is now able to un-nest the CSS in order to let everything render correctly.

### Roles and Members are now Colored in the Permissions Settings
Fermi now colors the roles/members within the permissions settings of guilds and channels

### 28k lines of code
Fermi is now 28k lines of TypeScript long now! (not including whitespace and comments)
While not a super helpful metric, it's always interesting to see how it's growing and maturing!

### Minor improvements
* Update manifest slightly
* Change the order of elements on the home page
* Changed default notification Volume to 20%
* Play object loads immediately instead of waiting for first interaction
* Reduce logging
* When a user sets their pfp, it should now update everywhere in Fermi as its set
* Localuser will now prevent duplicate user lookups when resolving a user object by ID
* Added a light blur in background when the user clicks on something
* Added text for when the client loads so the user knows if the client has loaded even if the loading screen doesn't slide away for some reason
* General grammar improvements in internal documents
	- [thanks to ErrorOliver2's pull request](https://github.com/MathMan05/Fermi/pull/157)
* Search GUI is much better
* In channel permissions it now says `permissions` instead of `roles`
* Trusted domains are now saved and are available in the settings
* Copy ID is now in the Permissions menu
* https:// is now assumed if provided a domain with nothing else [Implements](https://github.com/MathMan05/Fermi/issues/165)
* 3 stickers per row by making them slightly more narrow

### Bug fixes
* 0 Volume is no longer overridden with 100
* The default text in channels no longer overwrites the can't send messages here message
* Collects box content instead of relying on box content being captured by the markdown class.
* Fixed slight issue where the User class was incorrectly typed in a spot
* Empty context menus no longer error
* Mobile sidebar fix
	- [thanks to ygg2's pull request](https://github.com/MathMan05/Fermi/pull/153)
* Non-channel tabs could upload media [Fixes](https://github.com/MathMan05/Fermi/issues/155)
* Heading in settings wasn't clickable
* Fermi is now able to clear the unread status of deleted messages
* Dateline is now separate from the message [Fixes](https://github.com/MathMan05/Fermi/issues/156)
* Fixed error with multi removing some elements
* Clicking on blog posts in the settings now actually takes you to the blog
* Fermi now sets muted status correctly (this didn't effect Fermi before, but other clients)

### Mitigations
* nothing this week

### Discovered Spacebar Bugs
* nothing this week

### Spacebar fixes
* nothing this week

### The Best Way of Reporting Bugs/Feature Requests
If you want to be credited and have better chances of your ideas coming to life please [submit an issue on github](https://github.com/MathMan05/Fermi/issues)! This makes things easier for me as everything is in one place, and you can be credited in the blog posts as well via a link to the issue you have created!

If you guys have anything you'd like to see feel free to [open an issue](https://github.com/MathMan05/Fermi/issues/new) or say your ideas in the [Fermi Spacebar guild](https://fermi.chat/invite/USgYJo?instance=https%3A%2F%2Fspacebar.chat) or even the [Spacebar Discord Server](https://discord.gg/JDjMXTGeY9)
