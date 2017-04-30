---
layout: default
---

# Pork2b2tBot

This is a web overview of 2b2t. It's still under contruction, and a lot of things are broken or unimplemented. You can view the source code [here](https://github.com/DaMatrix/Pork2b2tBot).

The overview is run by a bot user (2pork2bot) and some stuff with websockets.

<iframe src="http://www.daporkchop.net/Pork2b2tBot/index.html" scrolling="no" style="border: 0; width: 100%; height: 1024px;" id="chatframe"></iframe>

## Known bugs

- Not all players show up in tab list

## Unimplemented (planned) features

- Chat viewing
- Chat sending/recieving (probably via /msg ingame, and a seperate iframe here)

## Credits

- torogadude for the name
- Steveice10 for making PacketLib and MCProtocolLib, this wouldn't be possible without you :D
- The guy who made [this](http://stackoverflow.com/a/30313558), for colored text
- The many people on StackExchange who helped me learn JavaScript for this

<script type="application/javascript">function resizeIFrameToFitContent( iFrame ) {iFrame.width  = iFrame.contentWindow.document.body.scrollWidth;iFrame.height = iFrame.contentWindow.document.body.scrollHeight;}  window.setInterval(function(){ resizeIFrameToFitContent(document.getElementById("chatframe")) }, 50);</script>