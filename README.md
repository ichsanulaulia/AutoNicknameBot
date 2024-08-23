<a href="https://top.gg/bot/1237341801094840350">
  <img src="https://top.gg/api/widget/1237341801094840350.svg">
</a>

# AutoNickname Discord Bot

AutoNickname is a powerful Discord bot designed to automate and manage nicknames for your server members. Whether it's changing nicknames for new members or automatically updating them when members receive new roles, AutoNickname handles it all effortlessly.

## Support the Development
Do you love what AutoNickname does? If you’d like to see more features and continuous improvements, you can support the development of this bot in various ways:

### Join as a Supporter
You can join our growing community of supporters on GitHub. Your support helps keep this project alive and thriving!

[Become a GitHub Sponsor](https://github.com/sponsors/ichsanulaulia)

### Donate via Cryptocurrency
If you prefer to support us via cryptocurrency, donations are greatly appreciated in BTC, USDT, LTC, and other major coins. Your contributions help cover the costs of hosting, maintenance, and further development.

**BTC:**  `1FPUUZqRxE75PbzYtLR622HkCsvZT1AoDs`  
**USDT TRC 20:** `TR8Hus7mzvJEJuJeYnJBBy9YM6JV95pFaE`

No matter how you choose to support, we’re incredibly grateful for your help in making AutoNickname better for everyone!

<h5 style="color: #999; padding: 0 20px 25px; border-radius: 5px; background: #0c091a;">
Your generosity directly impacts the bot's development and helps us continue to provide this service to the community. Thank you!
</h5>
<h5 style="color: #999; padding: 0 20px 25px; border-radius: 5px; background: #0c091a;">
With this bot, you can manage your discord server members' nicknames easily and automatically!
</h5>

## [Tutorial Video](https://www.youtube.com/watch?v=y8N5qQ3LqV0)
[Watch Tutorial](https://www.youtube.com/watch?v=y8N5qQ3LqV0)

### Overview
AutoNickname is a Discord bot designed to simplify nickname management within your server. Whether you want to change nicknames for new members or automatically adjust them based on roles, AutoNickname has you covered.

### Key Features
1. **Nickname Customization:**
   - Change nicknames for new members or when members get any roles.
   - Add prefixes or suffixes to nicknames using `{uname}` for the user's username and `{gname}` for the global name.
   - Logging System: use `/log` to set the status and channel for logging.

2. **Auto Nickname for New Members:**
   - Automatically set nicknames for users when they join your server.
   - Use `/nick-join` with `{uname}` for the user's username and `{gname}` for the global name.

3. **Role-Based Nicknames:**
   - Modify nicknames when someone gets specific roles. Use the command `/role-add` (for one role) or `/role-add-all` to add each role in your server.
   - Example: If someone named OZORAA receives the "Moderator" role, their nickname becomes "OZORAA Moderator."

## Important Notes
- **Role Hierarchy:**
  - The bot cannot change nicknames if the target person's role is higher than the bot's role.
  - To fix this, ensure the bot's role is positioned at the top.
- **Server Owner Nicknames:**
  - The bot cannot change the server owner's nickname due to Discord rules.
- **Support Server:**
  - Join the support server for error logs and assistance.

[AutoNickname Bot on Top.gg](https://top.gg/bot/1237341801094840350)

<h5 style="color: #999; padding: 0 20px 25px; border-radius: 5px; background: #0c091a;">
- The bot will not be able to change nicknames if the role of the person it wants to change is higher than the bot's role itself or if the role to be set is higher than the bot's role. (You must move the bot's role to the top to fix this issue.)

- If you are the server owner, the bot can't change your nickname! (This cannot be fixed due to Discord rules.)

- If you don't want to set logs on your server, please join the support server; all error logs are available there.

**PLEASE DON'T BE LAZY TO WATCH THE TUTORIAL VIDEO. EVERYTHING ABOUT AUTONICKNAME IS EXPLAINED THERE.**
</h5>

# AutoNickName Command List

## General Commands
- **/info-bot**
  - **Description:** Shows all bot-related information in this guild.
  
- **/avatar**
  - **Description:** Get the avatar of a specified user.
  - **Options:**
    - `user` (optional): The user whose avatar you want to view.

- **/help**
  - **Description:** Displays help information about the bot and its commands.

- **/info-server**
  - **Description:** Get detailed information about a user or the server.
  
- **/getnick**
  - **Description:** Retrieve a nickname similar to the one given to new joining members.
  - **Permissions Required:** Manage Nicknames

## Role Management Commands
- **/role-add**
  - **Description:** Add a specific role to the AutoNickname feature.
  - **Options:**
    - `role`: The role to add.
    - `name`: A custom name that includes `{uname}` for username and `{gname}` for global name, e.g., "Auto {uname}".
  - **Permissions Required:** Manage Guild

- **/role-add-all**
  - **Description:** Automatically add all roles in your server to the AutoNickname feature.
  - **Options:**
    - `nickname_type` (optional): Choose between "Username" or "GlobalName".
  - **Permissions Required:** Manage Guild

- **/role-remove**
  - **Description:** Remove a specific role from the AutoNickname feature.
  - **Options:**
    - `role`: The role to remove.
  - **Permissions Required:** Manage Guild

- **/role-remove-all**
  - **Description:** Automatically remove all roles in your server from the AutoNickname feature.
  - **Permissions Required:** Manage Guild

## AutoNickname Configuration Commands
- **/nick-join**
  - **Description:** Set a nickname template for members who join the guild.
  - **Permissions Required:** Manage Guild

- **/status-join**
  - **Description:** Toggle the AutoNickname feature for members who join the guild.
  - **Permissions Required:** Manage Guild

- **/status-role**
  - **Description:** Toggle the AutoNickname feature for when members gain or lose roles.
  - **Permissions Required:** Manage Guild

- **/status-welcome-dm**
  - **Description:** Toggle the welcome message feature sent via DM.
  - **Permissions Required:** Manage Guild

- **/message-welcome-dm**
  - **Description:** Set a custom welcome message that is sent via DM.
  - **Permissions Required:** Manage Guild

## Logging Commands
- **/log**
  - **Description:** Set up and configure logging channels and features for AutoNickname.
  - **Permissions Required:** Manage Guild

## Role Position for AutoNickname

![AutoNickname for Only Joined Members](https://github.com/ichsanulaulia/AutoNicknameBot/blob/master/img/ForAutoJoinNickname.gif)
*The first GIF demonstrates the AutoNickname feature for new members. This is the recommended setup role position if your server has a members role.* 

![AutoNickname for Members Roles and Joined Members](https://github.com/ichsanulaulia/AutoNicknameBot/blob/master/img/ForAutoNickname%20For%20Members%20Roles.gif)
*The second GIF ensures that the setup role position for changes nicknames based on members' roles (when a role is added or removed). Note that the bot will not be able to change nicknames if the target role or the role being set is higher than the bot's role itself. To resolve this, you must move the bot's role to the top like this.*
- If you are the server owner, the bot can't change your nickname! (This cannot be fixed due to Discord rules.) 

# AutoBot
A Discord bot for changing username for joined members And Change NickName When Members Get Any Roles
one of the bots that has a feature to count calculating time streaming on voice channel, showing leaderboars of streamers , and this bot is very good to use for servers such as game community or any server
[Tutorial Is Here](https://youtu.be/h1Um5Ui8b90)

# AutoTranslate
Discord bot with the main feature of automatically detecting languages and translating to languages based on Reaction Messages
With this bot, users can easily translate messages into different languages to improve communication in Discord

# AutoPing
discord bot that has the main feature to ping and monitor all links that have been inputted into the bot database. quite useful for anyone who wants to monitor their website, or just monitor any website or any bot server , interval every minutes.

