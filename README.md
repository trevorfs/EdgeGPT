# DiscordBot-EdgeGPT
> ### Using Bing on discord bot, your Microsoft account needs to be able to access Bing first.
> 
## Update
> ### 2023/4/26 : Create a separate chat for each user.
> ### 2023/4/24 : Now can generate images by Creative style.
> ### 2023/4/19 : When old Cookies expire, the bot can set new Cookies directly by prefix command.
   
## Features

<details>
   <summary>
   
   ### Slash command

   </summary>
   
* bing: `/bing [message]`

   | USE_SUGGEST_RESPONSES: True  (can change in file ```config.yml```) |
   |---|
  ![edgegpt](https://i.imgur.com/cLPL156.png)

   | USE_SUGGEST_RESPONSES: False (can change in file ```config.yml```) |
   |---|
  ![edgegpt](https://i.imgur.com/yK3P9Kt.png)
  
  | conversation style: Creative |
   |---|
  ![creative_style](https://i.imgur.com/IIzRsqj.png)
  
* bing image creator: `/create_image [prompt]`
  
  ![bingimage.png](https://i.ibb.co/0rxNbnk/2023-04-07-191036.png)
 
* conversation style (default balanced): `/switch_style [style]`
  
  ![style.png](https://i.ibb.co/54KMWKH/2023-04-07-200312.png)

* reset: `/reset`

  ![reset](https://i.imgur.com/AG5qQ1F.png)
</details>

<details>
   <summary>
   
   ### Prefix command (available only to bot owner)

   </summary>
   
 * `!unload [file_name_in_cogs_folder]`: Disable command from the specified file.
 * `!load [file_name_in_cogs_folder]`: Enable the command from the specified file.
 
   ![load & unload](https://i.imgur.com/spsyAEG.png)
  
 * `!clean`: Empty discord_bot.log file.
 * `!getLog`: Get discord_bot.log file. Real-time tracking of the bot's operating status.
   
   ![getLog](https://i.imgur.com/LHX4yWV.png)
 
 * `!upload [.txt_file]`: Because Bing Cookies will expire, so this command can set new Cookies directly and restart bot. You just need to copy bing cookies and past,                           the Cookies will auto convert to .txt file.
 
   ![upload](https://i.imgur.com/UN1Ac7N.png)
</details>

## Install
```
pip install -r requirements.txt
```

## Usage
1. Rename the file`.env.dev`to`.env`, then open it and edit it.
   ```
   DISCORD_BOT_TOKEN=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
   ```
   
2. Get Bing authentication.
   * Install the cookie editor extension for Chrome or Firefox.
   * Go to [bing.com](http://bing.com/chat)
   * Click "Export" on the bottom right.
   * Paste your cookies into a file `cookies.json`

4. Start run your bot, hosted locally or on a server.

   -> Recommended Free Servers: [fly.io](https://fly.io/)

## Credits
* EdgeGPT - [https://github.com/acheong08/EdgeGPT](https://github.com/acheong08/EdgeGPT)
* BingImageCreator - [https://github.com/acheong08/BingImageCreator](https://github.com/acheong08/BingImageCreator)
* other - [https://github.com/Zero6992/chatGPT-discord-bot](https://github.com/Zero6992/chatGPT-discord-bot)

## Contributors

This project exists thanks to all the people who contribute.

 <a href="https://github.com/FuseFairy/DiscordBot-EdgeGPT/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=FuseFairy/DiscordBot-EdgeGPT" />
 </a>
