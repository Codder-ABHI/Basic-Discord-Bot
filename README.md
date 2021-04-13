# Basic Discord Bot

Installation

```sh
npm i discord.js
```

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
