# SyntaxError-Identifier-bot-has-already-been-declared
help me 


const Discord = require ('discord.js')
const bot = new Discord.Client({intents:["GUILDS",["GUILD_MESSAGES"]]});
const Levels = require('discord-xp')
const bot = new Client({ intents: [ Intents.FLAGS.GUILD_MESSAGES]});

Levels.setURL("")

Client.login('')

bot.on("ready", bot => {
    console.log('Bot is Online !')

})

bot("message", async message => {
    const prefix = '!dxp';

    const args = message.content.slice(prefix.length).trim().split(/+/g);
    const command = args.shift().toLowerCase();


     const randomXp = Math.floor(math.random() * 9) + 1;
     const hasLevelUp = await Levels.fetch(message.author.id, message.guild.id);
     if(hasLevelUp){
        const user = await Levels.fetch(message.author.id, message.guild.id, randomXp);
        message.channel.send(`You are currently level **${use.level}**!`)

    }

    if(command === "leaderboard" || command === "lb") {
        const rawLeaderboard = await Levels.fetchLeaderboard(message.guild.id, 5);
        if (rawLeaderboard.length < 1) return reply("Nobody's in leaderboard yet.");

       const leaderboard = Levels.computeLeaderboard(bot,rawleaderboard);

       const lb = leaderboard.map(e => `${e.position}. ${e.username}#${e.discriminator}\nLevel: ${e.level}\nXP: ${e.xp.toLocaleString()}`);
       message.channel.send(`${lb.join("\n\n")}}`)

    }
    Client.login(token)
})
