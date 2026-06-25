# BedWars2023 PunchToDeposit

> A seamless BedWars resource deposit plugin for Minecraft servers — punch a chest, deposit everything. That's it.

## Overview

**BedWars PunchToDeposit** is a lightweight yet powerful Spigot plugin built on top of [BedWars2023](https://github.com/tomkeuper/BedWars2023) that transforms how players interact with chests during BedWars games. Instead of opening a chest and manually moving items, players simply **punch a team chest or ender chest** to instantly deposit all matching resources from their inventory / making gameplay faster, smoother, and more competitive.

Designed with performance in mind, the plugin reads item totals **directly from the chest inventory** rather than relying on fragile in-memory counters, ensuring the deposit total displayed to players is always accurate and no matter how many times they deposit or withdraw.


## Features

- **Punch-to-Deposit** — Left-click any team chest or ender chest to instantly deposit all matching items from your inventory
- **Accurate Total Display** — Shows the real item count inside the chest after each deposit, not a running counter that can drift out of sync
- **Team Chest & Ender Chest Support** — Both chest types handled with separate configurable messages
- **Per-Arena Lifecycle** — Deposit state is automatically cleared when a game ends, with no carryover between matches
- **Configurable Messages** — Full control over deposit messages, colors per team, and placeholders via `messages.yml`
- **Anti-Spam Cooldown** — Built-in deposit cooldown to prevent accidental double-deposits
- **Hologram Support** — Optional floating "PUNCH TO DEPOSIT" hologram rendered above chests during active games
- **Arena-Aware** — Fully integrated with the BedWars2023 arena lifecycle (game start, end, player join/leave)
- **bStats Metrics** — Anonymous usage metrics powered by bStats


## Installation

1. Download the latest `Bedwars-PunchToDeposit-1.0.jar` from the [Releases](../../releases) page
2. Place it in your server's `plugins/` folder
3. Make sure [BedWars2023](https://github.com/tomkeuper/BedWars2023) is installed
4. Restart the server
5. Configure `messages.yml` and `config.yml` generated in `plugins/BedWars2023-Deposit/`


## Requirements

| Requirement | Version |
|---|---|
| Java | 11+ |
| Spigot / PaperSpigot | 1.8.8 – 1.21 |
| BedWars2023 | 5.0.0+ |
