---
layout: default
---

# PorkBot
A Discord bot

<a href="https://discordapp.com/oauth2/authorize?client_id=287894637165936640&scope=bot&permissions=37022784" target="_blank">Invite</a>

<a href="https://github.com/DaMatrix/PorkBot" target="_blank">Source code</a>

## Commands

#### Categories

[General](#general)

[Minecraft](#minecraft)

[Music](#music)

[Misc](#misc)

# General<a name="general"></a>

| Command name | Description                                                            | Usage                                          | Example                                                                | Note                                                          |
|--------------|------------------------------------------------------------------------|------------------------------------------------|------------------------------------------------------------------------|---------------------------------------------------------------|
| help         | Sends a link to this page                                              | `..help`                                       | `..help`                                                               |                                                               |
| invite       | Sends the bot invite link                                              | `..invite`                                     | `..invite`                                                             |                                                               |
| botinfo      | Gets some information about the bot                                    | `..botinfo`                                    | `..botinfo`                                                            |                                                               |
| ping         | Shows the bot's latency                                                | `..ping`                                       | `..ping`                                                               |                                                               |


# Minecraft<a name="minecraft"></a>

| Command name | Description                                                            | Usage                                          | Example                                                                | Note                                                          |
|--------------|------------------------------------------------------------------------|------------------------------------------------|------------------------------------------------------------------------|---------------------------------------------------------------|
| mcface       | Shows the face of a Minecraft skin                                     | `..mcface <username>`                          | `..mcface Notch`                                                       |                                                               |
| mchead       | Shows the head of a Minecraft skin                                     | `..mchead <username>`                          | `..mchead Notch`                                                       |                                                               |
| mcskin       | Shows a Minecraft skin                                                 | `..mcskin <username>`                          | `..mcskin Notch`                                                       |                                                               |
| skinsteal    | Shows a raw Minecraft skin                                             | `..skinsteal <username>`                       | `..skinsteal Notch`                                                    |                                                               |
| mcuuid       | Gets the UUID associated with a Minecraft username                     | `..mcuuid <player name>`                       | `..mcuuid Notch`                                                       |                                                               |
| offlineuuid  | Gets the UUID that a player would have on an offline-mode server       | `..offlineuuid <player name>`                  | `..offlineuuid Notch`                                                  |                                                               |
| mcping       | Pings a Minecraft server and gets some info about it                   | `..mcping <ip>` OR `..mcping <ip:port>`        | `..mcping 2b2t.org` OR `..mcping 2b2t.org:25565`                       |                                                               |
| mcmotd       | Gets the current MOTD of a Minecraft server                            | `..mcmotd <ip>` OR `..mcmotd <ip:port>`        | `..mcmotd 2b2t.org` OR `..mcmotd 2b2t.org:25565`                       |                                                               |
| mccount      | Gets the current player count on a Minecraft server                    | `..mccount <ip>` OR `..mccount <ip:port>`      | `..mccount 2b2t.org` OR `..mccount 2b2t.org:25565`                     |                                                               |
| mcicon       | Gets the icon of a Minecraft server                                    | `..mcicon <ip>` OR `..mcicon <ip:port>`        | `..mcicon 2b2t.org` OR `..mcicon 2b2t.org:25565`                       |                                                               |
| mclatency    | Gets the latency (ping) to a Minecraft server                          | `..mclatency <ip>` OR `..mclatency <ip:port>`  | `..mclatency 2b2t.org` OR `..mclatency 2b2t.org:25565`                 |                                                               |
| mcversion    | Gets a Minecraft server's version                                      | `..mcversion <ip>` OR `..mcverision <ip:port>` | `..mcversion 2b2t.org` OR `..mcversion 2b2t.org:25565`                 | Returns protocol version number too                           |
| mcquery      | Gets more information about a Minecraft server                         | `..mcquery <ip>` OR `..mcquery <ip:port>`      | `..mcquery bepis.pepsi.team` OR `..mcquery mc.glowstone.net:25565`     | Only works if `enable-query` is `true` in `server.properties` |
| peping       | Pings a Minecraft: Pocket Edition server and gets some info about it   | `..peping <ip>` OR `..peping <ip:port>`        | `..peping play.2p2e.net` OR `..peping play.2p2e.net:19132`             |                                                               |
| pequery      | Queries a Minecraft: Pocket Edition server and gets more info about it | `..pequery <ip>` OR `..pequery <ip:port>`      | `..pequery play.2p2e.net` OR `..pequery play.2p2e.net:19132`           | Only works if `enable-query` is `true` in `server.properties` |
| pecount      | Gets the current player count on a Minecraft: Pocket Edition server    | `..pecount <ip>` OR `..pecount <ip:port>`      | `..pecount play.2p2e.net` OR `..pecount play.2p2e.net:19132`           |                                                               |
| pelatency    | Gets the latency (ping) to a Minecraft: Pocket Edition server          | `..pelatency <ip>` OR `..pelatency <ip:port>`  | `..pelatency play.2p2e.net` OR `..pelatency play.2p2e.net:19132`       |                                                               |
| peversion    | Gets a Minecraft: Pocket Edition server's version                      | `..peversion <ip>` OR `..peversion <ip:port>`  | `..peversion play.2p2e.net` OR `..peversion play.2p2e.net:19132`       |                                                               |
| pemotd       | Gets the current MOTD of a Minecraft: Pocket Edition server            | `..pemotd <ip>` OR `..pemotd <ip:port>`        | `..pemotd play.2p2e.net` OR `..pemotd play.2p2e.net:19132`             |                                                               |


# Music<a name="music"></a>

| Command name | Description                                                            | Usage                                          | Example                                                                | Note                                                          |
|--------------|------------------------------------------------------------------------|------------------------------------------------|------------------------------------------------------------------------|---------------------------------------------------------------|
| play         | Adds a track to the queue by link                                      | `..play <link>`                                | `..play https://youtu.be/ytWz0qVvBZ0`                                  | May be a playlist. [Supported links](#music-supported-links)  |
| play         | Adds a track to the queue using YouTube search                         | `..play <search terms>`                        | `..play diggy diggy hole`                                              |                                                               |
| play         | Adds a track to the queue using the given platform's search            | `..play <platform> <search terms>`             | `..play soundcloud dboyd lazy dayze`                                   | Case-insensitive. [Supported platforms & shortcuts](#music-supported-platforms) |
| playlist     | Adds all the tracks from a given plain-text playlist                   | `..playlist <url>`                             | `..playlist https://pastebin.com/raw/EjJ1JkF8`                         | [Small example](https://pastebin.com/EjJ1JkF8), [Big example](https://cloud.daporkchop.net/random/music/httplist.txt) |
| queue        | Shows the songs in the queue                                           | `..queue [page]`                               | `..queue` OR `..queue 3`                                               |                                                               |
| shuffle      | Makes the queue ignore the order of tracks in the queue                | `..shuffle`                                    | `..shuffle`                                                            | Queue will remain shuffled until disabled with `..ordered`    |
| ordered      | Makes the queue be played back in order (default)                      | `..ordered`                                    | `..ordered`                                                            |                                                               |
| skip         | Skips the currently playing song                                       | `..skip`                                       | `..skip`                                                               |                                                               |
| stop         | Clears the playlist and stops playing                                  | `..stop`                                       | `..stop`                                                               |                                                               |


### Supported link types<a name="music-supported-links"></a>

- YouTube videos
- SoundCloud tracks
- BandCamp tracks
- Vimeo videos
- Twitch streams
- Beam tracks
- Raw media files: `.mp3`, `.ogg`, `.flac`, `.wav`, `.mp4`, `.mkv`

- YouTube playlists
- SoundCloud playlists
- BandCamp albums
- PPLST playlists ([example](https://cloud.daporkchop.net/random/music/list.pplst))


### Supported search platforms (& shortcuts)<a name="music-supported-platforms"></a>

- YouTube (shortcuts: `yt`)
- SoundCloud (shortcuts: `sc`, `soundc`)


# Misc<a name="misc"></a>

| Command name | Description                                                            | Usage                                          | Example                                                                | Note                                                          |
|--------------|------------------------------------------------------------------------|------------------------------------------------|------------------------------------------------------------------------|---------------------------------------------------------------|
| dice         | Rolls a die!                                                           | `..dice` OR `..dice <count`                    | `..dice` OR `..dice 3`                                                 |                                                               |

