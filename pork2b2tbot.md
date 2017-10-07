---
layout: default
---

# Pork2b2tBot

This is a web overview of 2b2t. It's still under contruction, and a lot of things are broken or unimplemented. You can view the source code [here](https://github.com/DaMatrix/Pork2b2tBot).

Please report any bugs or feature requests at [here](https://github.com/DaMatrix/Pork2b2tBot/issues). Thanks!

The overview is run by a bot user (2pork2bot) and some stuff with websockets.

<iframe src="http://www.daporkchop.net/Pork2b2tBot/index.html?address=repo.daporkchop.net&port=8888" scrolling="no" style="border: 0; width: 100%;" id="chatframe"></iframe>

## Help

Here's a few simple things to rembember:
- All actions, ingame or on the site, have a 5 second cooldown.
- When sending a message ingame, the bot only sends 1 message per second to avoid getting kicked. Just because you don't recive a reply instantly, doesn't mean it won't happen! Try waiting a few seconds.
- Inactive users on the site are logged out after 10 minutes, and won't recive messages.
- Accounts that aren't logged in with for 30 days are invalidated, and will have to be registered again (not that it's that difficult lol)

When using the bot ingame, you'll need to rembember this syntax:

`/msg 2pork2bot <target player name> <message to send>`

This command will send a message to a player logged into the website, by their name. Keep in mind that logged in users are automagically logged out after 10 minutes of inactivity.
An example can be seen here:

`/msg 2pork2bot torogadude hello there!`

This would send "hello there!" to torogadude, assuming he's logged in on the site.

On the site (here), you can do as follows:

### Registration

1. Enter your IGN in the first text box, and your password you want to use in the second one.
2. Press "Log in". You'll be sent a command, that you need to send ingame on 2b2t. Keep in mind that this confirmation command expires after 10 minutes or the bot restarting, but you can always run step 1 again :P
3. After running the command 2pork2bot will send you back here. Refresh the page and use the same IGN and password, you'll get a new interface.

### Sending chat from the site

After registering and logging in, you'll be able to send messages.

1. Enter the name of the user you want to message in the first text box.
2. Enter your message in the second one.
3. Press "Send"
4. The user will get your message ingame! (if they're logged in to 2b2t, that is :P)

### Changing your password

If you forget your password to log into the site, you can join 2b2t and issue the following command:

`/msg 2pork2bot changepass <new password>`

I don't feel any further explaination is required for this.

## Known bugs

- Ping in tab list shows incorrectly

## Unimplemented (planned) features

- Graphs! (player online times, when players are most active, etc.)
- Desktop notifications when a DM is recieved

## Credits

- torogadude for the name
- Steveice10 for making PacketLib and MCProtocolLib, this wouldn't be possible without you :D
- The guy who made [this](http://stackoverflow.com/a/30313558), for colored text
- The many people on StackExchange who helped me learn JavaScript for this
- [This](https://github.com/Caligatio/jsSHA), for client-side password hashing


<script type="application/javascript">function resizeIFrameToFitContent( iFrame ) { iFrame.height = iFrame.contentWindow.document.body.scrollHeight; }  window.setInterval(function(){ resizeIFrameToFitContent(document.getElementById("chatframe")) }, 50);</script>