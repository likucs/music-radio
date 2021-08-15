# VCMusicPlayer v3.0

- An Telegram Bot to Play Radio/Music in Channel or Group Voice Chats.
- A Telegram Bot to Play Audio in Voice Chats With Youtube and Deezer support.
- Supports Live streaming from YouTube.

## How to deploy 

Click the below button to watch the video tutorial on deploying

<a href="https://youtu.be/FKaAU4Pr2bw"><img src="https://img.shields.io/badge/How%20To%20Deploy%20v3.0%20Latest-blue.svg?logo=Youtube"></a>
<a href="https://youtu.be/FKaAU4Pr2bw"><img src="https://img.shields.io/youtube/views/FKaAU4Pr2bw?style=social">

<a href="https://youtu.be/FGZr-V2lCo8"><img src="https://img.shields.io/badge/How%20To%20Deploy%20v2.0%20Old-blue.svg?logo=Youtube"></a>
<a href="https://youtu.be/FGZr-V2lCo8"><img src="https://img.shields.io/youtube/views/FGZr-V2lCo8?style=social">


## Deploy to Railway

<p><a href="https://railway.app/new/template?template=https%3A%2F%2Fgithub.com%2Flikucs%2FRadioPlayerV3&envs=API_ID%2CAPI_HASH%2CBOT_TOKEN%2CSESSION_STRING%2CCHAT%2CLOG_GROUP%2CADMINS%2CADMIN_ONLY%2CMAXIMUM_DURATION%2CSTREAM_URL%2CREPLY_MESSAGE&optionalEnvs=LOG_GROUP%2CADMIN_ONLY%2CMAXIMUM_DURATION%2CSTREAM_URL%2CREPLY_MESSAGE&API_IDDesc=Your+Telegram+API_ID+get+it+from+my.telegram.org%2Fapps&API_HASHDesc=Your+Telegram+API_HASH+get+it+from+my.telegram.org%2Fapps&BOT_TOKENDesc=Bot+token+of+your+bot%2C+get+from+%40Botfather&SESSION_STRINGDesc=Session+string%2C+use+%40genStr_robot+to+generate+pyrogram+session+string&CHATDesc=ID+of+Channel+or+Group+where+the+Bot+plays+Radio%2FMusic%2FYouTube+Lives&LOG_GROUPDesc=ID+of+the+group+to+send+playlist+if+CHAT+is+a+Group%2C+if+channel+then+leave+blank&ADMINSDesc=ID+of+Users+who+can+use+Admin+commands+%28for+multiple+users+seperated+by+space%29&ADMIN_ONLYDesc=Change+it+to+%27True%27+If+you+want+to+make+%2Fplay+commands+only+for+admins+of+CHAT.+By+default+%2Fplay+is+available+for+all.&MAXIMUM_DURATIONDesc=Maximum+duration+of+song+to+be+played+using+%2Fplay+command&STREAM_URLDesc=URL+of+Radio+station+or+Youtube+Live+video+url+to+stream+with+%2Fradio+command&REPLY_MESSAGEDesc=A+reply+message+to+those+who+message+the+USER+account+in+PM.+Make+it+blank+if+you+do+not+need+this+feature.&MAXIMUM_DURATIONDefault=15&ADMIN_ONLYDefault=False&STREAM_URLDefault=https://youtu.be/5qap5aO4i9A&REPLY_MESSAGEDefault=Hello Sir, I'm a bot to play radio/music/youtube live on telegram voice chat, not having time to chat with you 😂!"> <img src="https://img.shields.io/badge/Deploy%20To%20Railway-blueviolet?style=for-the-badge&logo=railway" width="200""/></a></p>

NOTE: Make Sure You Have Started A Voice Chat In Your Channel/Group Before Deploying!

## NOTE:

- Make sure you have started a VoiceChat in your Group before deploying.

## Deploy to Heroku

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/likucs/music-radio)

### Deploy to VPS

```sh
git clone https://github.com/LushaiMusic/VCMusicPlayer
cd VCMusicPlayer
pip3 install -r requirements.txt
# <Create Variables appropriately>
python3 main.py
```

# Configs Vars:
1. `API_ID` : Get From my.telegram.org
2. `API_HASH` : Get from my.telegram.org
3. `BOT_TOKEN` : @Botfather
4. `SESSION_STRING` : Generate From here [![GenerateStringName](https://img.shields.io/badge/repl.it-generateStringName-yellowgreen)](https://replit.com/@ZauteKm/GenerateStringSession)
5. `CHAT` : ID of Channel/Group where the bot plays Music.
6. `LOG_GROUP` : Group to send Playlist, if CHAT is a Group
7. `ADMINS` : ID of users who can use admin commands.
8. `ARQ_API` : Get it for free from [@ARQRobot](https://telegram.dog/ARQRobot), This is required for /dplay to work.
9. `STREAM_URL` : Stream URL of radio station or a youtube live video to stream when the bot starts or with /radio command.
10. `MAXIMUM_DURATION` : Maximum duration of song to play.(Optional)
11. `REPLY_MESSAGE` : A reply to those who message the USER account in PM. Leave it blank if you do not need this feature. 
12. `ADMIN_ONLY` : Pass `Y` If you want to make /play and /dplay commands only for admins of `CHAT`. By default /play and /dplay is available for all.

- Enable the worker after deploy the project to Heroku
- Bot will starts radio automatically in given `CHAT` with given `STREAM_URL` after deploy.(24*7 Music even if heroku restarts, radio stream restarts automatically.)  
- To play a song use /play as a reply to audio file or a youtube link.
- Use /play <song name> to play song from youtube and /dplay <song name> to play from Deezer.
- Use /help to know about other commands.

**Features**

- Playlist, queue
- Supports Live streaming from youtube
- Supports both deezer and youtube to search songs.
- Play from telegram file supported.
- Starts Radio after if no songs in playlist.
- Automatically downloads audio for the first two tracks in the playlist to ensure smooth playing
- Automatic restart even if heroku restarts.

#### Support
Join Now Telegram [VC Music Live Sets](https://t.me/c/1481808444/131)

## Requirements

- Python 3.6 or higher.
- A
  [Telegram API key](https://docs.pyrogram.org/intro/quickstart#enjoy-the-api)
  and a Telegram account.
- [FFmpeg Python](https://www.ffmpeg.org/)
- Telegram [String Session](http://t.me/UsePyrogramBot) of the account.
- Userbot Needs To Be Admin In The Channel or Group.
- Must Start A Voice Chat In Channel/Group Before Running The Bot.

## License
```sh
VC Music Player, Telegram Voice Chat Userbot
Copyright (C) 2021  Zaute Km

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>
```

## Credits

- [Zaute Km](https://github.com/Zaute-Km) [Dev]
- [Dash Eclipse](https://github.com/dashezup) [For tgvc_userbot]
- [Marshal X](https://github.com/MarshalX) [For pytgcalls]
