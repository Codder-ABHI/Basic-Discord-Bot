# Basic Discord Bot

Installation

Use npm init and it will create a package.json file

```sh
npm init
```

Now Make a File called `index.js` 

```sh
npm i discord.js
```

Get your bot token from Discord Developer Portal

```javascript
const Discord = require("discord.js");
const client = new Discord.Client();
 

let prefix = "!";// or use the prefix that you want 

client.on("message", (message) => {

  if (!message.content.startsWith(prefix) || message.author.bot) return;
 
  if (message.content.startsWith(prefix + "ping")) {
    message.channel.send("pong.");
 
  }
});
 
client.login("your bot token");
```
To Start the Bot Use

```sh
node index.js
```
