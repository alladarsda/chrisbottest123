# A discord bot made with JavaScript and the discord.js-commando library

[![forthebadge](https://forthebadge.com/images/badges/made-with-javascript.svg)](https://forthebadge.com)

Please drop a ⭐ if you find this repo/bot useful :)

### Installing the dependencies

`npm i`

### Usage

Make a config.json file in the root directory of the project and add:

```
{
  "prefix": "!",  // You can change the prefix to whatever you want it doesn't have to be - !
  "token": "Your-Bot-Token",
  "tenorAPI": "tenor-API-key",
  "newsAPI": "news-api-key",
  "youtubeAPI": "youtube-api-key",
  "yandexAPI": 'yandex-api-key"
}
```

I run the bot on a debian 9 environment so it might not work as intended on other operating systems, if you need a guide on how to install node.js on debian 9 or ubuntu I will link one in the resources down below. Moreover, the music command is still under development, so it might break.

Also, no matter what operating system you have, make sure [ffmpeg](https://www.ffmpeg.org/download.html) and [python 2.7](https://www.python.org/downloads/) are installed.

### Commands

- Music

|   Command    |   Description | Usage   |
| -----             |    ------           | -----          |
|!play              | Play any song or playlist from youtube, you can do it by searching for a song by name or song url or playlist url             | !play darude sandstorm    |
|!pause              | Pause the current playing song   | !pause          |
|!resume              |Resume the current paused song  |!resume           |
|!leave              | Leaves voice channel if in one              |!leave           |
|!remove              | Remove a specific song from queue by its number in queue |!remove 4           |
|!queue             | Display the song queue              |!queue           |
|!shuffle              |Shuffle the song queue               |!shuffle           |
|!skip              |Skip the current playing song               |!skip           |
|!skipall              |Skip all songs in queue               | !skipall          |
|!skipto              |Skip to a specific song in the queue, provide the song number as an argument               | !skipto 5          |

- Misc

|   Command    |   Description | Usage     |
| -----        |    ------     | -----     |
| !cat             | Get a cute cat picture              | !cat             |
| !fortune             | Get a fortune cookie tip              |   !fortune        |
| !global-news             | Latest headlines from reuters, you can change the news source to whatever news source you want, just change the source in line 13 in global-news.js or ynet-news.js| !global-news         |
| !random             | Generate a random number between two provided numbers              |!random 0 100           |
| !reddit             | Replies with 5 top non nsfw subreddit posts   | !reddit askreddit          |
| !say             |  Make the bot say anything             |!say Lorem Ipsum       |
| !translate             | Translate to English(for now) from any supported language using yandex translation service|!translate ありがとう           |
| !whomademe             |  Info about me and the repo       | !whomademe          |

- Gifs

|   Command    |   Description | Usage     |
| -----        |    ------     | -----     |
|!animegif              | Get an anime related gif by a query               |!animegif one punch man           |
|!gif              | Get any gif by a query              |!gif labrador           |
|!gintama              |Replies with a random gintama gif               |!gintama              |
|!jojo              |eplies with a random jojo gif               |!jojo             |

- Guild

|   Command    |   Description | Usage     |
| -----        |    ------     | --------------    |
| !ban             | Bans a tagged member              | !ban @johndoe          |
| !create-text-channel             | Creates a text channel              | !create-text-channel music-discussion          |
| !create-voice-channel             | Creates a new voice channel              | !create-voice-channel Music Channel         |
| !kick             | Kicks a tagged member              | !kick @johndoe          |
| !prune               | Delete up to 99 recent messages              | !prune 50          |

### Resources

[Get a Tenor API key here](https://tenor.com/developer/keyregistration)

[Get a NewsAPI API key here](https://newsapi.org/)

[How to get a Youtube API key](https://developers.google.com/youtube/v3/getting-started)

[Get a Yandex API key here](https://translate.yandex.com/developers/keys)

[Installing node.js on debian](https://www.digitalocean.com/community/tutorials/how-to-set-up-a-node-js-application-for-production-on-debian-9)

### Contributing

Fork it and submit a pull request!
Anyone is welcome to suggest new features and improve code quality!

### Tasks

- [ ] Improve code quality
- [ ] Write more guild commands
- [ ] Improve music quality
