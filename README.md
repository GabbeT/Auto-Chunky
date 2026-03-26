# Auto Chunky

A lightweight, server-side Fabric utility mod for Minecraft 1.21.1 that automatically manages the [Chunky](https://modrinth.com/plugin/chunky) pre-generation mod based on player activity.

## About
When running a Minecraft server, pre-generating the world is great, but it can cause massive lag if players join while it's running. Auto Chunky solves this by automatically pausing the generation when players are online and resuming it when the server is empty.

## Features
- **Auto-Pause:** Instantly executes `/chunky pause` behind the scenes when a player connects.
- **Auto-Resume:** Starts a 2-minute countdown when the last player disconnects. If the server remains empty, it executes `/chunky continue`.
- **Admin Commands:** Use `/autochunky toggle` to turn the automation ON/OFF, and `/autochunky status` to check its current state (Requires OP/Permission Level 2).

## Requirements & Recommended Setup
- Minecraft 1.21.1
- Fabric Loader **0.18.5+** & Fabric API
- [Chunky](https://modrinth.com/plugin/chunky) (Server-side)
- **Tip:** Set `continueOnRestart` to `true` in your Chunky config. This makes Chunky start automatically with the server, letting Auto Chunky handle the pausing when someone joins.

## How to build from source
If you want to compile the mod yourself, you will need Java 21 installed.

1. Clone the repository:
   ```bash
   git clone [https://github.com/GabbeT/Auto-Chunky.git](https://github.com/GabbeT/Auto-Chunky.git)
