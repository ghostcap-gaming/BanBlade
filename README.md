# BanBlade: Next generation ban management for Counter Strike 2

Brought to you by **GhostCap**.

BanBlade is the next generation of ban management for Counter Strike 2, designed exclusively for Discord. Say goodbye to old school systems like Sourcebans++ and embrace the future with BanBlade. This revolutionary system provides an intuitive and real-time experience without the need for a clunky web interface that gets outdated every year. Players can check their ban status directly within Discord, ensuring swift and clear communication.

We've developed this so it's as lightweight as possible, while also making it easy to install on most peoples existing game server stack. Please keep in mind this is in beta. Our vision is to architect a system that will not only carry CS2 servers through the next 10 years, but also to ensure it's structured flexibly. This way, if you ever decide to transition to another platform or create your own web panel, accessing your bans will be seamless and hassle-free.

**Everything here is subject to change!**

## 🚀 Current Features

- **Directly Ban/Unban from Discord**: No need to log into any separate systems.
- **RBAC**: Simply assign permissions to roles in Discord, no need to add any further rules.
- **Server Mods No More**: Operate seamlessly without the need for any mods on your CS2 server.
- **Auto punishment tracking**: Never worry about "have I punished this person before", everything is handled automatically with incremental punishments.
- **Supports Multiple Servers**: One bot, multiple servers. Centralize your control.
- **No Rcon Requirement**: BanBlade works without the need for rcon.
- **Integration with Panels**: Directly talks to Pterodactyl and WISP panels using their application API for more security.

Possible Future Updates
- Companion plugin to help communicate with the database and monitor in game chat using AI.
- Communications bans. These would be the same way Valorant handles things as the existing gag/mute way is antiquated. This would auto support incremential punishments if a player keeps offending. 

## 📜 Requirements

- **MySQL 8.0** or above
- **Python Bot Hosting**
- **Pterodactyl or WISP Panel**

## 📜 Commands
All commands are ran through Discord right now as there is no companion plugin.

/check - Will check the punishment status of your linked steam account.
/check <steamid or url> - Can check the punishment status of any player.
/gamepunish <steamid or url> - Will automatically punish the player with the next incremental punishment you have set and kick them from the server.
/gameban <steamid> - Will instantly permanent ban the player and kick the from the server.

## 📥 Installation

**Note**: BanBlade is currently in invite-only mode. Please await further details on public releases.
