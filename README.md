# BanBlade: Next generation game ban management for gaming communities

BanBlade is the next generation of ban management for gaming communities, designed exclusively for Discord. Say goodbye to old school systems like Sourcebans++ or litebans, and embrace the future with BanBlade. This revolutionary system provides an intuitive and real-time experience without the need for a clunky web interface that gets outdated every year. Players can check their ban status directly within Discord, ensuring swift and clear communication.

![screenshot](https://i.imgur.com/93j4Vsi.png)

The goal is to be simple to use for any staff member and user, no matter their experience level. Everyone will be shown the same information to ensure everyone is on the same page with how and why they were punished. 

We've developed this so it's as lightweight as possible, while also making it easy to install on most peoples existing game server stack.

**Everything here is subject to change!**

## 🚀 Current Features

- **Directly Ban/Unban from Discord**: No need to log into any separate systems.
- **RBAC**: Simply assign permissions to roles in Discord, no need to add any further rules.
- **Server Mods Not Required**: BanBlade is designed to work without the need for a modded server giving you the basic ability to manage any server.
- **Automatic punishment tracking**: Never worry about "have I punished this person before", everything is handled automatically with incremental punishments.
- **Supports Multiple Servers**: One bot, multiple servers. Centralize your control.
- **Automatic Communications Bans**: Is a player being toxic in chat? Silence or ban toxic players instantly without admin intervention.
- **No Rcon Requirement**: BanBlade works without the need for rcon.
- **Integration with Panels**: Directly talks to Pterodactyl panel using their client API for more security than RCON.

Possible Future Updates
- Companion plugins to help communicate with the database and monitor in game voice chat using AI.
- Live Alerts: Get alerted on Discord when a player is being toxic on your servers.

## 📜 Requirements

- **MySQL 8.0** or above
- **Python Bot Hosting**
- **Rcon Access** (Optional*)
- **Pterodactyl** (Optional*)
- **Perspective API** (Optional)

* You must use either Rcon or Pterodactyl

## 📜 Commands
Here are the commands for Discord. Anyone is able to run the /check commands but only DIscord roles with permissions will be able to interact with punishments.
 
/check - Will check the punishment status of your linked steam account.
/check <steamid or url> - Can check the punishment status of any player.
/gamepunish <steamid or url> <reason> - Will automatically punish the player with the next incremental punishment you have set and kick them from the server.
/gameban <steamid or url> <reason> - Will instantly permanent ban the player and kick them from the server.

## 📥 Installation

**Note**: BanBlade is currently in invite-only mode. Please await further details on public releases.

These are basic instructions on how the BanBlade install will work.

First create a bot for your Discord server. You can call this what you want to match your community brand. (Exact roles TBA)

Installation is handled by a Pterodactyl egg. Simply install the egg to your server, and it will pull the latest version of BanBlade from GitHub to your server. You would then be able to create a database within that instance to hold all your ban data. 
  
From there, you simply modify the settings.json and credentials.json with your servers. No need to worry about manually updating. These files are not overwritten on updates, however new config files are created on your server instance if those files have changed on GitHub.  
  
We plan to have BanBlade work on existing configs within the same version number (ie. version 1 configs should work with all versions, regardless of what's inside)

You can also run BanBalde on its own with anything that supports Python. Simply run banblade.py and connect it to your own MySQL database. You won't receive automatic updates on restart this way.
