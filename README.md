# KygekClearConsole

[![Discord](https://img.shields.io/discord/735439472992321587.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/CXtqUZv)

**NOTICE:** This plugin branch is for PocketMine-MP 4. If you are looking for the PocketMine-MP 3 version of this plugin, please visit the [main](https://github.com/KygekTeam/KygekClearConsole/tree/main) branch.

A PocketMine-MP plugin to clear server console using command. This plugin is roughly equivalent to `cls` command on Windows or `clear` command on Linux.

This plugin is not planned to be released on Poggit, because it may break Rule A1 or A2 (see [Poggit Rules](https://poggit.pmmp.io/rules.edit) for more information, and remember to use common sense!).

## ❔ How Does This Plugin Works

This plugin clears the console when the `clearconsole` command (Alias: `cc`) gets executed. This plugin prints `\e[H\e[J` character to console to clear the console. This plugin ensures the command will only show and work on console by using `CommandEvent` to capture the command and cancelling the event to prevent unexpected outputs (e.g. Unknown command) if the sender is from the console.

## ✅ Features

- Only works in console
- Command gets hidden in command suggestions and help page (Player)
- Sends unknown command message whenever a player tries to execute the command
- API to clear the console (`ClearConsole::clear()`)

## 🔧 Installation

1. 🔽 Download the latest version from GitHub Releases or Poggit CI below:
    - Stable version (Recommended for most users): [Latest](https://github.com/KygekTeam/KygekClearConsole/releases/latest) | [All releases](https://github.com/KygekTeam/KygekClearConsole/releases)
    - Build version (Only recommended for advanced users): [Poggit CI](https://poggit.pmmp.io/ci/KygekTeam/KygekClearConsole/~)
2. 📁 Drop the downloaded `KygekClearConsole.phar` plugin file into your PocketMine-MP server's `plugins` directory.
3. 🔄 Restart your server and you're ready to test the plugin!

## 🔐 Commands & Permissions

| Command | Description | Aliases |
| --- | --- | --- |
| `/clearconsole` | Clears server console | `/cc` |

## 🧾 Planned Features

Nothing for now. You can request for a feature to be added in a future update [here](https://github.com/KygekTeam/KygekClearConsole/issues)!

## ➕ Additional Info

KygekClearConsole is a PocketMine-MP plugin by KygekTeam and licensed under **GPL-3.0**.

- Join our Discord server [here](https://discord.gg/CXtqUZv) for latest news and support from KygekTeam.
- If you found bugs or want to give suggestions, please visit [here](https://github.com/KygekTeam/KygekClearConsole/issues) or join our Discord server.
- We accept all contributions! If you want to contribute please make a pull request in [here](https://github.com/KygekTeam/KygekClearConsole/pulls).