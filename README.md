# Advanced Achievements

Part of the Cobbleworks Minecraft plugin ecosystem.

Source section copied from the main plugin collection repository:
https://github.com/BerndHagen/Minecraft-Server-Plugins

## Overview

An advanced achievement system that tracks player progress for various task types (block breaking, crafting, mob kills, etc.) and provides highly configurable rewards. All progress and claim status are stored persistently per player. The plugin architecture allows for custom extensions via API.

### Core Features:
- **Progress Tracking:** Real-time tracking for all task types (block breaking, crafting, mob kills, etc.)
- **Reward System:** Economy (Vault), items, XP, titles, commands – all configurable per achievement
- **Database:** Supports MySQL and SQLite, including asynchronous load/save
- **GUI:** Inventory-based GUI with pages, navigation, and progress display (BossBar/ActionBar)
- **API:** Add custom achievements and triggers via API
- **Messages:** All messages and prefixes are fully customizable (YAML)
- **Prerequisites:** Achievements can depend on other achievements
- **Sound/Firework:** Unlocks can optionally play a sound and firework

### Administrative & Player Commands:

| Command | Description |
|---------|-------------|
| `/achievementadmin reload` | Reloads all configuration files and achievements |
| `/achievementadmin reset <player>` | Resets a player's progress |
| `/achievementadmin give <player> <id>` | Manually awards an achievement |
| `/achievementadmin create` | Starts an interactive creation dialog in chat |
| `/achievementadmin edit <id>` | Edits an existing achievement |
| `/achievementadmin delete <id>` | Permanently deletes an achievement |
| `/achievementadmin list [category] [page]` | Lists achievements with filtering and pagination |
| `/achievementadmin gui` | Opens the achievements GUI |
| `/achievementadmin info <id>` | Shows all details for an achievement |
| `/achievementadmin progress [id]` | Shows progress for all/specific achievements |
| `/achievementadmin help` | Shows all available commands |

**Aliases:** `/achadmin`, `/ach` (all subcommands as above)

## License

This project is licensed under the MIT License.