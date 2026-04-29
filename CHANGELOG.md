# Changelog

All notable changes to Advanced Achievements will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [Unreleased]

## [1.0.2] - 2026-04-29

Advanced Achievements v1.0.2 expands the task system and improves command-driven achievement creation with stronger runtime handling.

### New Tasks And Command Improvements

- **Expanded Task Coverage**: Added additional task-type support so more gameplay actions can be tracked through achievements
- **Command Flow Improvements**: Refined command/session handling for creating and managing achievements with the newer task definitions
- **Configuration Alignment**: Updated achievement configuration data to match the expanded task model and runtime processing

**Note:** If you encounter any bugs or issues, please don't hesitate to open an [issue](https://github.com/Cobbleworks/Advanced-Achievements-Plugin/issues). For any questions or to start a discussion, feel free to initiate a [discussion](https://github.com/Cobbleworks/Advanced-Achievements-Plugin/discussions) on the GitHub repository.

## [1.0.1] - 2026-04-28

Advanced Achievements v1.0.1 delivers stability improvements and maintenance fixes following the initial release.

### Stability And Maintenance

- **Runtime Safety**: Improved error handling and runtime stability across high-player-count environments
- **General Refinements**: Applied maintenance updates for long-running servers

**Note:** If you encounter any bugs or issues, please don't hesitate to open an [issue](https://github.com/Cobbleworks/Advanced-Achievements/issues). For any questions or to start a discussion, feel free to initiate a [discussion](https://github.com/Cobbleworks/Advanced-Achievements/discussions) on the GitHub repository.

## [1.0.0] - 2026-04-01

Advanced Achievements v1.0.0 is the initial release, delivering a fully configurable achievement system with 12 task types, a reward engine, GUI browser, database integration, and a developer API.

### Achievement System

- **12 Task Types**: Tracks block breaking, item pickup, mob kills, crafting, fishing, eating, enchanting, trading, mining, breeding, taming, and player death — each supporting `ANY` targets or specific material/entity names
- **Prerequisite Chains**: Achievements can require other achievements to be unlocked first for multi-step progression
- **Hidden Achievements**: Achievements can be hidden from the list and GUI until unlocked

### Reward Engine

- **Five Reward Types**: Items, XP, economy money (Vault), server commands with `{player}` and `{uuid}` placeholders, and title messages — all defined in `achievements.yml`

### User Interface

- **Inventory GUI**: Paginated achievement browser with real-time progress bars, colour-coded states (locked/unlocked/claimed), and click-to-claim rewards
- **Chat Creation Wizard**: Step-by-step guided flow for creating achievements without editing YAML
- **Broadcast Notifications**: Server-wide broadcast message on achievement unlock, configurable per achievement
- **Sound And Firework Effects**: Configurable sound and optional firework at the player's location on unlock
- **Progress Display**: Optional ActionBar or BossBar progress bar with configurable refresh interval

### Database And Persistence

- **Dual Backend**: Supports SQLite for single-server setups and MySQL for multi-server or network environments
- **Asynchronous I/O**: All database reads and writes run on background threads

### Developer Integration

- **Java API**: Full `AchievementAPI` for external plugins to create achievements, query progress, grant unlocks, and add progress programmatically

**Note:** If you encounter any bugs or issues, please don't hesitate to open an [issue](https://github.com/Cobbleworks/Advanced-Achievements/issues). For any questions or to start a discussion, feel free to initiate a [discussion](https://github.com/Cobbleworks/Advanced-Achievements/discussions) on the GitHub repository.
