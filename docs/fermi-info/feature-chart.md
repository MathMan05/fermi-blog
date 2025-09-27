This is a chart to try and help compare all of the features of clients and the server, to let users know what is and isn't working yet. This should help make comparisons easier.

| Feature | [Spacebar Server](https://github.com/spacebarchat/server) | [Fermi](https://fermi.chat) | [React Client](https://app.spacebar.chat/) |
| --- | ---- | --- | --- |
| DMs | ✅ | [✅🛈]("Not all features are supported, but most of the work is done") | ❌ |
| Per channel drafts | N/A | ✅ | ❌ |
| Embeds | ✅ | ✅ | ✅ |
| Reactions | [✅🛈]("There's currently a bug where all of the people who've reacted to a message are sent with the message instead of just the first few") | ✅ | ❌ |
| File uploading | [✅🛈]("Only old style file uploading is supported") | ✅ | ✅ |
| Voice chats | [✅🛈]("Not enabled by default is known to have issues on some platforms") | [✅⏳🛈]("Most of the way there, works in both chromium and firefox") | ❌ | 
| Video chats | [✅🛈]("Not enabled by default is known to have issues on some platforms") | [⏳🛈]("Only chromium works right now") | ❌ | 
| Live streams | [✅🛈]("Not enabled by default is known to have issues on some platforms") | [⏳🛈]("Only chromium works right now") | ❌ | 
| Logging in | ✅ | ✅ | ✅ | 
| Creating accounts | ✅ | ✅ | [✅🛈]("Does not have a TOS box") | 
| Deleting accounts | ✅ | ✅ | ❌ | 
| Logging out | ✅ | ✅ | ✅ | 
| Friend requests | ✅ | [⏳🛈]("Menu needs reworking") | ❌ |
| Notifications | N/A | ✅ | ❌ |
| Push Notifications | ❌ | [❌🛈]("While possible with the web, there's currently no server support from spacebar") | ❌ |
| Gateway reconnection[🛈]("This allows clients to resume without restarting the software") | [✅🛈]("The RESUME event is not supported so it's not as graceful as one would hope") | ✅ | [❌🛈]("It is supported in the code, but there's currently a bug where it causes the client to make repeated requests to the server causing undue strain so is disabled") |
| Profile editing | ✅ | ✅ | [⏳🛈]("Only setting the pfp is supported") |
| Profile viewing | ✅ | [✅⏳🛈]("Profiles mostly work but aren't complete yet") | [⏳🛈]("Only some parts of profiles work") |
| Mobile support | N/A | [✅⏳🛈]("It works, though more work could be done to improve it") | ❌ |
| Channel reordering | ✅ | ✅ | ❌ |
| Channel creation | ✅ | ✅ | ✅ |
| Permission settings | ✅ | [✅⏳🛈]("Only role permissions are currently supported") | ❌ |
| Replying | [✅🛈]("Does not support no ping replies") | ✅ | ❌ |
| Webhooks | ✅ | ✅ | [❌🛈]("Can only view messages from them, can't manage them at all") |
| Creating bots | ✅ | ✅ | [❌🛈]("Likely will depend on an external bot panel for this instead") |
| GIF support | [✅🛈]("Does not support discord style gifs") | ✅ | [⏳🛈]("Only supports seeing gifs") |
| Custom Emoji | ✅ | ✅ | [⏳🛈]("Works in some spots but not others") |
| Managing custom Emoji | ✅ | ✅ | ❌ |
| Guild discovery | ✅ | ✅ | ❌ |
| Setting guild icons | ✅ | ✅ | ❌ |
| Guild banners | ✅ | ✅ | [❌]("Does not support viewing or setting them") |
| Member list | [⏳🛈]("Sometimes does not want to work due to a bug and sends it in the wrong order")| [✅🛈]("Does caching to help fill out the member list") | [✅🛈]("Does not cache the member list and relies on the server \(this is not incorrect)")|
| Guild search | [⏳🛈]("Sends the count of items sent rather than the count of items that match") | ✅ | ❌ |
| Category creation | ✅ | ✅ | [❌🛈]("Does not support it, though it does support creating channels within them") |
| Leaving guilds | ✅ | ✅ | [✅🛈]("There is a bug if you're the owner of a guild where you can't leave it and it does not present you with the option to delete it") |
| Deleting guilds | ✅ | ✅ | ❌ |
| 2FA[🛈]("Two factor authentication") | [✅🛈]("Only supports time based codes") | [✅🛈]("Needs to gain the feature to download backup codes") | [⏳🛈]("Only supporting logging in with it, but not creating the 2FA") |
| Status | [⏳🛈]("Does not support setting it when a session is already active and has a few bugs with it") | [✅🛈]("Does not fully work due to the server issues") | [⏳🛈]("Only supports viewing") |
| Markdown | N/A | ✅ | ✅ |
| Editing messages | [✅🛈]("Link Embeds have a bug where they'll duplicate and reactions don't persist") | ✅ | ❌ |
| Message pinning | ✅ | ✅ | ❌ |
| Embed creation | N/A | ❌ | ❌ |
| Account switching | N/A | ✅ | ❌ |
| Account recovery | [✅🛈]("Requires email to be set up") | [✅🛈]("Not available on all instances") | ❌ |
| Setting new password | ✅ | ✅ | ❌ |
| Setting new email | ✅ | ✅ | ❌ |
| Setting discriminator | ✅ | ✅ | ❌ |
| Creating invites | ✅ | ✅ | [⏳🛈]("Can create the codes, but the invite URL is lacking")|
| Guild profiles | ✅ | ✅ | ❌ |
| Templates | [❌🛈]("Doesn't work due to a lot of bugs") | [⏳🛈]("Likely works, not throughly tested") | ❌ |
| Stickers | ✅ | ✅ | ❌ |
| NSFW channels | ✅ | ✅ | [❌🛈]("It just looks like normal channels with no warning") |
| Rules channel | ✅ | ✅ | [❌🛈]("It just looks like a normal channel") |
| Translations | ✅ | ✅ | ❌ |
| Channel visibility[🛈]("showing/hiding channels based on if the user can see them") | N/A | ✅ | ✅ |
| Autofill | N/A | [✅🛈]("Does not currently support roles, everyone or here") | ❌ |
| Components | [❌🛈]("Sometimes they can be uploaded, but they don't work") | [❌🛈]("Would implement if the server had support for them") | ❌ |
| Interactions | ❌ | ❌ | ❌ |
| Polls | [❌🛈]("Can be sent, but they don't work") | ❌ | ❌ |
| Resume[🛈]("Makes reconnecting faster and more seamless") | ❌ | [⏳🛈]("Likely works though untested") | ❌ |
| Threads | ❌ | ❌ | ❌ |
| Community channel types | ❌ | ❌ | ❌ |
| Registration tokens[🛈]("A special single use token that allows for someone to join an instance and bypass captchas, and registration being disabled") | ✅ | ✅ | ❌ |
| Profile badges | ✅ | ✅ | ❌ |
