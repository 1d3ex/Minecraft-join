# Join/Quit Messages (Skript)

A simple [Skript](https://skripthub.net/) for Minecraft servers that disables default join/quit messages and replaces them with a clean, custom broadcast message.

## Features
* **Join Event:** Removes the default `[Player] joined the game.` message and broadcasts `👤 [Player] has entered.` to the entire server.
* **Quit Event:** Removes the default `[Player] left the game.` message and broadcasts `👤 [Player] has left the game.` to the entire server.

## Code
```skript
on join:
	set join message to ""
	broadcast "&7👤 %player% has entered."
	
on quit:
	set quit message to ""
	broadcast "&7👤 %player% has left the game."
