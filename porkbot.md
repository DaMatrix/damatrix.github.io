---
layout: default
---

# PorkBot
A Minecraft-focused Discord bot

[Invite](https://discordapp.com/oauth2/authorize?client_id=287894637165936640&scope=bot&permissions=8)

## Commands

| Command name | Description                                                          | Usage                                     | Example                                                                | Note                                                        |
|--------------|----------------------------------------------------------------------|-------------------------------------------|------------------------------------------------------------------------|-------------------------------------------------------------|
| help         | Sends a link to this page                                            | `..help`                                  | `..help`                                                               |                                                             |
| invite       | Sends the bot invite link                                            | `..invite`                                | `..invite`                                                             |                                                             |
| say          | Makes the bot send a message                                         | `..say <message you want to say>`         | `..say Hello World!`                                                   |                                                             |
| mcavatar     | Shows the face of a Minecraft skin                                   | `..mcavatar <username>`                   | `..mcavatar Notch`                                                     | Also works with UUID instead of username                    |
| mchead       | Shows the head of a Minecraft skin                                   | `..mchead <username>`                     | `..mchead Notch`                                                       | Also works with UUID instead of username                    |
| mcskin       | Shows a Minecraft skin                                               | `..mcskin <username>`                     | `..mcskin Notch`                                                       | Also works with UUID instead of username                    |
| mcping       | Pings a Minecraft server and gets some info about it                 | `..mcping <ip>` OR `..mcping <ip:port>`   | `..mcping 2b2t.org` OR `..mcping 2b2t.org:25565`                       |                                                             |
| mcmotd       | Gets the current MOTD of a Minecraft server                          | `..mcmotd <ip>` OR `..mcmotd <ip:port>`   | `..mcmotd 2b2t.org` OR `..mcmotd 2b2t.org:25565`                       |                                                             |
| mccount      | Gets the current player count on a Minecraft server                  | `..mccount <ip>` OR `..mccount <ip:port>` | `..mccount 2b2t.org` OR `..mccount 2b2t.org:25565`                     |                                                             |
| mcicon       | Gets the icon of a Minecraft server                                  | `..mcicon <ip>` OR `..mcicon <ip:port>`   | `..mcicon 2b2t.org` OR `..mcicon 2b2t.org:25565`                       |                                                             |
| mcquery      | Gets more information about a Minecraft server                       | `..mcquery <ip>` OR `..mcquery <ip:port>` | `..mcquery home.daporkchop.tk` OR `..mcquery home.daporkchop.tk:25565` | Only works if `enable-query` is true in `server.properties` |
| peping       | Pings a Minecraft: Pocket Edition server and gets some info about it | `..peping <ip>` OR `..peping <ip:port>`   | `..peping play.2p2e.tk` OR `..peping play.2p2e.tk:19132`               |                                                             |
| mcstatus     | Gets the status of Mojang servers                                    | `..mcstatus`                              | `..mcstatus`                                                           |                                                             |
| mcuuid       | Gets the UUID associated with a Minecraft username                   | `..mcuuid <player name>`                  | `..mcuuid Notch`                                                       |                                                             |
