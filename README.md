

ALL IN ONE BOT SCRIPT
MADE BY - 764546128204005436,716290028829147198

EVERYONE CAN U THIS REPO BY GIVING US CREDITS

## Categories 📚
- [x] Music & Filter
- [x] Fun
- [x] Anime
- [x] NSFW
- [x] Utility
- [X] Image
- [X] ChatBot
- [x] MODERATION
- 


HOW TO USE AND HOST THE BOT IN GLITCH

FIRST IMPORT THE PROJECT

THEN GO TO TERMINAL AND TYPE "npm install"

AND GO TO "config.json" AND ADD UR TOKEN AND API

{
    "prefix": "!",     
    "embedcolor": "EMBED_COLOUR", 
    "dev": "DEVELOPER_ID",       
    "token": "YOUR_PREFIX_HERE", 
    "database": "DATABASE",
    "ame_api": "AME_API HERE"     
    
}


TO CHANGE STATUS GO TO events/client AND WRITE UR STATUS 


const { PREFIX } = require('../../configs/config.json');
const moment = require('moment');
const chalk = require("chalk")

module.exports = async client => {
    let totalUsers = client.guilds.cache.reduce((users , value) => users + value.memberCount, 0);
    let totalGuilds = client.guilds.cache.size
    let totalChannels = client.channels.cache.size

    console.log(chalk.red`[${moment().format('YYYY-MM-DD HH:mm:ss')}] BOT: Active, Commands Loaded!`);
    console.log(chalk.red`[${moment().format('YYYY-MM-DD HH:mm:ss')}] BOT: ${client.user.username} Logged In!`);
    client.user.setPresence({ activity: { name: "YOUR STATUS HERE", type: "PLAYING" }, status: "idle" });
    console.log(chalk.blue`[${moment().format('YYYY-MM-DD HH:mm:ss')}] BOT: Now ` + totalChannels + ` channels, ` + totalGuilds + ` Servers and ` + totalUsers + ` serving  users!`);
}

AND LAST STEN GO TO TERMINAL AND TYPE NODE INDEX.JS AND UR BOT WILL BE ONLINE


IF U NEED ANY HELP DM - <@764546128204005436> AND <@716290028829147198>

IF U WANT TO BUY CUSTOM BOT/CUSTOM BOT REPO THEN JOIN THIS SERVER LINK - https://discord.gg/vEXkFZtx
