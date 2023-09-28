# ImperialsBot
 Minecraft bot using mineflayer to chat spam, safeguard bases and many other utility functions. 3D display using prismarine viewer of the bot

# Imperial Bot Setup Guide

This guide will help you set up and run your Minecraft bot using the provided JavaScript code and configuration file.

## Prerequisites

- [Node.js](https://nodejs.org) installed on your system.
- A text editor to modify the configuration file.

## Installation

1. Download the bot source files (JavaScript code and configuration files) from [Release](https://github.com/tanishisherewithhh/ImperialsBot/releases) or clone the github repository by putting this into your terminal or command prompt:
```
gh repo clone tanishisherewithhh/ImperialsBot
```
3. Run the `install.bat` file to install the necessary dependencies. This can be done by double clicking and running the `install.bat` OR typing `install.bat` in the terminal and pressing enter.

## Configuration

Open the `config.json` file in a text editor to modify the bot's settings. Here's what each setting does:

- `ip`: The IP address of the Minecraft server you want the bot to connect to.
- `username`: The username for the bot.
- `password`: The password for the bot to /register or /login.
- `version`: The version of Minecraft that the server is running.
- `port`: The port number for the local web server that displays the bot's view and controls.
- `blacklist`: An array of usernames that the bot should ignore.
- `antiafk`: If set to true, the bot will move around randomly to avoid being kicked for being AFK.
- `autoreconnect`: If set to true, the bot will automatically try to reconnect if it gets disconnected.
- `reconnectdelay`: The delay (in seconds) before attempting to reconnect after being disconnected.
- `securityguard`: If set to true, the bot will alert when a player enters its render distance.
- `firstperson`: If set to true, the web view will be in first-person mode. If false, it will be in third-person mode.
- `killsuicide`: If set to true, the bot will use `/kill` command for suicide. If false, it will try to find other ways (like lava or flint and steel).
- `killaura.killaura`: If set to true, Killaura will be enabled.
- `killaura.mob`: If set to true, Killaura will target mobs.
- `killaura.player`: If set to true, Killaura will target players.
- `log.messages`: If set to true, chat messages will be logged.
- `log.whispers`: If set to true, whispers will be logged.
- `log.kicks`: If set to true, kick messages will be logged.
- `log.death`: If set to true, death messages will be logged.
- `log.errors`: If set to true, error messages will be logged.
- `chat.bypass`: If set to true, a random string will be added to the end of the chat messages to bypass spam filters.
- `chat.bypasslimit`: The length of the random string added for spam filter bypassing.
- `chat.random`: If set to true, messages from the message list will be chosen randomly. If false, they'll be chosen sequentially.
- `chat.delay`: The delay (in seconds) between each chat message sent by the bot when spamming is enabled.
- `chat.messages`: An array of messages that the bot can send when spamming is enabled.
- `webhookUrl`: The URL of a Discord webhook that the bot can send messages to.
### Make sure you follow the JSON format inorder for it to be used without any errors.
Example Edit:
```json
{
 "ip": "8b8t.me",
 "username": "tanishisherewith",
 "password":"pro1927A",
 "version": "1.19.4",
 "port": "3000",
 "blacklist": ["User1", "User2"],
 "antiafk":true,
 "autoreconnect":true,
 "reconnectdelay": "4",
 "securityguard": true,
 "firstperson": false,
 "killsuicide": true,
  "killaura":{
    "killaura": true,
    "mob": false,
    "player": true
  },
  "log":{
    "messages": true,
    "whispers": true,
    "kicks": true,
    "death": false,
    "errors": true
  },
"chat":{
 "bypass": false,
 "bypasslimit":"0",
 "random": true,
 "delay": "7",
  "messages": [
    "My message 1 ",
    "Imperials  ",
    "On",
    "Top  "
  ]
},
"webhookUrl":"https://discord.com/api/webhooks/1156536070859653220/KTizv1dy_be3qsJpsc15BCu2gysgcFWUH3k2WFjnlEYW4u48bXf_pgA6Vnk0SB-LJ3YVZ1"
}
```

## Running

To start the bot, run the `start.bat` file by double clicking and running the `start.bat` OR typing `start.bat` in your terminal and pressing enter.
 
## Usage

Once running, you can interact with your bot through a web interface available at http://localhost: (whatever port number you specified in your configuration) (Example: http://localhost:3000). This interface allows you to control your bot's movements and send chat messages.

## Troubleshooting

If you encounter any issues while setting up or running your bot, check if there are any error messages in your terminal. These messages can often provide clues about what's going wrong.

If you're still having trouble, you may want to check that all your settings in your configuration file are correct (especially your server IP and version), and that all necessary dependencies were installed correctly.

For any FAQ or issues you can directly address them to the [issue](https://github.com/tanishisherewithhh/ImperialsBot/issues) page or contact me via discord `tanishisherewith`


# Imperial Bot Features

This bot is built using several powerful libraries that give it a wide range of capabilities:

## Mineflayer

Mineflayer is a high-level Minecraft bot API. It's capable of doing everything you might want a bot to do, including navigating the world, fighting mobs, mining, crafting, and more.

## Cracked Account Support

This bot supports cracked accounts or non premium minecraft accounts or offline mode accounts

## Auto Auth

This bot automatically `/register` and `/login` with the password given in `config.json` file

## Mineflayer PvP

The Mineflayer PvP plugin allows the bot to engage in combat with other players or mobs. It can automatically target and attack entities within its range.

## Mineflayer Pathfinder

The Mineflayer Pathfinder plugin enables the bot to navigate the Minecraft world. It can find paths to specific locations, avoid obstacles, and even handle complex tasks like traversing mazes.

## Prismarine Viewer

Prismarine Viewer is used to provide a web-based view of what the bot sees in the game. This can be useful for debugging or just for watching what the bot is doing. It can be set to either first-person or third-person view.

## Discord Webhook Connection

The bot can send messages to a Discord channel via a webhook. This can be used to relay chat messages from the Minecraft server to Discord, send alerts or updates about what the bot is doing, or for any other communication needs.

## Anti-AFK

The bot has an anti-AFK feature that makes it move around randomly to avoid being kicked from the server for being idle.

## Auto Reconnect

If the bot gets disconnected from the server for any reason, it can automatically attempt to reconnect after a specified delay.

## Killaura

Killaura is a combat feature that automatically attacks entities within a certain range. This can be configured to target players, mobs, or both.

## Spamming

The bot can send chat messages at regular intervals. These messages can be chosen randomly or sequentially from a list, and a random string can be appended to bypass spam filters.

Remember that while these features are powerful, they should be used responsibly and in accordance with the rules of the server you're playing on.
