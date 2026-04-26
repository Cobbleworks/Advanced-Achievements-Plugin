<p align="center">
  <img src="images/plugin-logo.png" alt="Advanced Achievements" width="128" />
</p>
<h1 align="center">Advanced Achievements</h1>
<p align="center">
  <b>A comprehensive achievement system for Minecraft servers.</b><br>
  <b>Custom rewards, progress tracking, and persistent database integration.</b>
</p>
<p align="center">
  <a href="https://github.com/Cobbleworks/Advanced-Achievements/releases"><img src="https://img.shields.io/github/v/release/Cobbleworks/Advanced-Achievements?include_prereleases&style=flat-square&color=4CAF50" alt="Latest Release"></a>&nbsp;&nbsp;<a href="https://github.com/Cobbleworks/Advanced-Achievements/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue?style=flat-square" alt="License"></a>&nbsp;&nbsp;<img src="https://img.shields.io/badge/Java-17+-orange?style=flat-square" alt="Java Version">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Minecraft-1.21+-green?style=flat-square" alt="Minecraft Version">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Platform-Spigot%2FPaper-yellow?style=flat-square" alt="Platform">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square" alt="Status">
</p>

Advanced Achievements is an open-source Minecraft plugin that provides a comprehensive achievement system for Spigot and Paper servers. Originally developed for a private Minecraft server, the plugin tracks player progress across a wide range of task types including block breaking, crafting, mob kills, and many more. All progress and claim status are stored persistently per player, and the system is designed for deep configurability so server administrators can tailor rewards, messages, and unlock conditions to their exact needs.

### **Core Features**

- **Progress Tracking:** Real-time tracking for all task types including block breaking, crafting, mob kills, fishing, trading, and more
- **Reward System:** Supports economy rewards via Vault, item drops, experience points, title messages, and executable commands — all configurable per achievement
- **Database Integration:** Supports both MySQL and SQLite with full asynchronous load and save operations for minimal server impact
- **GUI Interface:** Inventory-based graphical menu with pages, navigation arrows, and live progress display via BossBar and ActionBar
- **API Support:** Server developers can register custom achievements and triggers via the plugin API
- **Fully Customizable Messages:** All chat messages, prefixes, unlock notifications, and item descriptions are configurable through YAML files
- **Achievement Prerequisites:** Achievements can depend on other achievements — players must unlock earlier goals before progressing
- **Sound and Firework Effects:** Unlock events can optionally trigger a configurable sound and a firework display at the player's location

### **Supported Platforms**

- **Server Software:** `Spigot`, `Paper`, `Purpur`, `CraftBukkit`
- **Minecraft Versions:** `1.21.5`, `1.21.6`, `1.21.7`, `1.21.8`, `1.21.9`, `1.21.10` and higher
- **Java Requirements:** `Java 17+`

### **Installation**

1. Download the latest `.jar` from the [Releases](https://github.com/Cobbleworks/Advanced-Achievements/releases) page
2. Stop your Minecraft server
3. Copy the `.jar` into your server's `plugins` folder
4. (Optional) Add Vault and a compatible economy plugin for economy rewards
5. Start your server — a default configuration folder is generated at `plugins/AdvancedAchievements/`

### **Administrative & Player Commands**

| Command | Description |
|---------|-------------|
| `/achievementadmin reload` | Reloads all configuration files and achievement definitions |
| `/achievementadmin reset <player>` | Resets all progress for the specified player |
| `/achievementadmin give <player> <id>` | Manually awards a specific achievement to a player |
| `/achievementadmin create` | Starts an interactive creation dialog in chat |
| `/achievementadmin edit <id>` | Opens an edit dialog for an existing achievement |
| `/achievementadmin delete <id>` | Permanently removes an achievement |
| `/achievementadmin list [category] [page]` | Lists all achievements with optional category filtering and pagination |
| `/achievementadmin gui` | Opens the achievements management GUI |
| `/achievementadmin info <id>` | Displays all details and configuration for a specific achievement |
| `/achievementadmin progress [id]` | Shows progress data for all or a specific achievement |
| `/achievementadmin help` | Lists all available commands with descriptions |

**Aliases:** `/achadmin`, `/ach`

### **Plugin Compatibility**

- **Economy:** Vault — required for economy-based rewards
- **Permissions:** LuckPerms, PermissionsEx, and any other Bukkit-compatible permission manager
- **Database:** MySQL for networked multi-server setups, SQLite for single-server deployments

### **License**

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

