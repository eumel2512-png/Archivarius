# Archivarius

**A lightweight Discord bot for World of Warcraft Forever guild communities.**

Archivarius makes useful WoW Forever reference information easy to access directly from Discord. It is a modular Python bot built around slash commands and links to established game-information sources.

## What it does

- **Dungeon and instance information** via `/ini`.
- **Item lookup** via `/item`.
- **General Wowhead search** via `/suche`, covering supported categories such as NPCs, recipes, quests, spells, zones and creatures.
- **Class guides** via `/klasse`.
- **Profession leveling guides** via `/beruf`.
- **Utility commands**, including dice rolling.

The exact information available depends on the connected external sources. Archivarius does not invent game data or use AI to interpret results.

## ForeverDB API access

We are interested in evaluating the ForeverDB API as an additional source for WoW Forever-specific reference data that may not be available through Wowhead Forever.

Potential use cases include retrieving supported item, NPC, recipe, quest, spell, profession and dungeon information on demand in response to Discord slash commands.

Requests would be user-triggered rather than continuously polling. Where ForeverDB data is displayed, the bot will provide the attribution and visible link required by ForeverDB's terms.

No API access or integration is claimed to be active at this stage. This repository describes the project and its intended use while API access is being explored.

## Technical overview

- Python 3.11
- discord.py 2.x
- Modular cog-based structure
- Asynchronous HTTP requests with aiohttp
- Hosted on a Pterodactyl-based game-server panel

## Project scope

Archivarius is a guild-community utility bot. It is not an AI assistant, character planner, inventory manager, gear optimizer or character database.

## Security

- Discord bot tokens and other credentials are kept outside the repository in environment configuration.
- Never commit `.env`, API keys, bot tokens or other secrets.
- Public project documentation must not contain private server or account credentials.

## Status

The bot is operational in its guild environment. Additional data-source integrations, including a possible ForeverDB connection, are subject to API access, documentation and compatibility checks.

---

*Project repository: [github.com/eumel2512-png/Archivarius](https://github.com/eumel2512-png/Archivarius)*
