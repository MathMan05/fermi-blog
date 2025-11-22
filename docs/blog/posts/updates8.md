---
date:
  created: 2025-11-21
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
description: This week I've gone through and implemented Mentions saving in the spacebar server, context menu stacking, and a lot of Spacebar fixes/improvements. 
---

# Mentions Saving, Context Menu Improvements and Tonnes of Spacebar Fixes
This week I've gone through and implemented Mentions saving in the spacebar server, context menu stacking, and a lot of Spacebar fixes/improvements. 
<!-- more -->
Not as many "flashy" features or fixes were really implemented this week, but that does not mean that work was not done, infact, a lot of work was done to try and polish the existing features and eliminate bugs in the current systems.

## this weeks updates

### Mention Count is now Implemented
I went in and actually implemented mention_count, so now when you get a ping or dm, the mentions will persist instead of going away with a refresh! (for those who are wondering, I implemented this in the server, don't worry, people who ping you while you're offline will still be counted!)

### Stacked context menus
Now context menus can "stack" where one menu is the primary menu, and the other menus that are bellow it can add items if they want to, so that way in the future if you right click a URL it can be made where the right click menu for the message you right clicked shows up, but also a button to copy the URL. This will allow for much better and more dynamic context menus.

### DMs Debugging
DMs are now much less bugfull, they should no longer bug out in most of the situations they did before, and groups are much more implemented now, with the icons actually displaying, the owner showing in the group list, you showing up in the list, and a tonne more, if you were having issues with this feature before, you should check it out again and see if the issues you were having before have been resolved!

### My Goals Going into the Future
I've been making Fermi for nearly 2 years now, and I'm starting to run out of things to actually implement into Fermi that don't require the server to start supporting it. You might notice that I've made many, many Spacebar improvements this week and I plan to keep this up ongoing into the future(it's honestly much easier than I thought it'd be lol, just make 50 branches and makes small-ish patches like that). I've gone through and fixes many of the bugs that've been pleaging the server and effecting Fermi users, and actually implemented a feature or two this week.

### Minor improvements
* Embeds titles without urls are no longer styled like links
* DM Group Dialog should now hide on submit
* DM and Channel names will now update live
* DM icons will update live
* Group DMs now support icons
* You will now see your own username in the group DMs menu
* Show group owner in groups
* More things check for groups vs dms instead of number of participents

[did this](https://github.com/MathMan05/Fermi/issues/173)

### Bug fixes
* Join Guild button no longer shows up if the guild isn't joinable
* Defaults to default notification value on Guild join
* More emojis are now processed correctly
* PFPs in embeds no longer look wonky
* Embeds now are respected on the send function
* Going to a bad channel should now not crash hopefully
* Notifications should no longer send resolving user and should instead just send the username
* Fix where emoji guild menu would show in the wrong z-order with pings
* The dming user field should now work more consistently
* New DMs should no longer look broken
* DMs should now sort live in send order
* Updating a DM no longer causes an internal error
* Channel updates are now assumed to be @me if not specified
* Sending a message now updates unreads and mentions in a better way

### Mitigations
* Mentions is now checked if it exists

### Discovered Spacebar Bugs
* Any guild could be joined via ID regardless if it was allowed

### Spacebar fixes
* [Made it so you can't join a guild via ID unless the guild allows it](https://github.com/spacebarchat/server/pull/1381)
* [Ignore bun lock file](https://github.com/spacebarchat/server/pull/1383)
* [Bots should not join default guilds by default now](https://github.com/spacebarchat/server/pull/1382)
* [Bots can't join guilds from discovery without a user authorizing it](https://github.com/spacebarchat/server/pull/1390)
* [Update unread state when welcome messages are sent](https://github.com/spacebarchat/server/pull/1384)
	- [Fixes](https://github.com/spacebarchat/server/issues/1336#event-21004887914)
* [Default notification values are now respected](https://github.com/spacebarchat/server/pull/1386)
	- [Fixes](https://github.com/spacebarchat/server/issues/1338)
* [Roles with only one color can now be edited again](https://github.com/spacebarchat/server/pull/1388)
* [Invalid pings no longer error the server](https://github.com/spacebarchat/server/pull/1387)
	- [Fixes](https://github.com/spacebarchat/server/issues/1326)
* [Webhooks without wait should work properly now](https://github.com/spacebarchat/server/pull/1393)
* [Embeds without a specified type are now assumed to be rich](https://github.com/spacebarchat/server/pull/1392)
* [Mention count](https://github.com/spacebarchat/server/pull/1394)
	- [more fixes](https://github.com/spacebarchat/server/pull/1395)
* [Groups now send icon and name](https://github.com/spacebarchat/server/pull/1397)
* [Keep track of group owners](https://github.com/spacebarchat/server/pull/1402)
* [Make member count more accurate](https://github.com/spacebarchat/server/pull/1391)

### The Best Way of Reporting Bugs/Feature Requests
If you want to be credited and have better chances of your ideas coming to life please [submit an issue on github](https://github.com/MathMan05/Fermi/issues)! This makes things easier for me as everything is in one place, and you can be credited in the blog posts as well via a link to the issue you have created!

If you guys have anything you'd like to see feel free to [open an issue](https://github.com/MathMan05/Fermi/issues/new) or say your ideas in the [Fermi Spacebar guild](https://fermi.chat/invite/USgYJo?instance=https%3A%2F%2Fspacebar.chat) or even the [Spacebar Discord Server](https://discord.gg/JDjMXTGeY9)
