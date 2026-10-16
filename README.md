# Hollow Descent Example Pack

Welcome to the **Example Pack** for **Hollow Descent**, a modular template pack designed to help creators understand how to build and structure custom content for the game. 

Whether you want to design custom rooms, configure unique tile mappings, or build entirely new floors, this pack serves as your foundational reference.

---

## Directory Structure

A valid pack requires a specific folder hierarchy and a `manifest.json` file at its root so the game's data loader can parse it correctly:

```text
example/
├── manifest.json
├── levels/
├── rooms/
└── tiles/

```

---

## 1. The Manifest (`manifest.json`)

The manifest file defines your pack's metadata, identification, versioning, licensing, and minimum required game version.

```json
{
  "id": "example",
  "name": "Example",
  "author": "Elrol",
  "version": "1.0.0",
  "min_game_version": "1.0.0",
  "license": "MIT",
  "is_core": false,
  "desc": "An example pack demonstrating data-driven asset loading for Hollow Descent."
}

```

---

## 2. Custom Content Folders

* **`levels/`** — Contains JSON files defining floor structures, room pools, and generation paths.
* **`rooms/`** — Contains layout data, grid footprints, exits, and entity/tile placement definitions for individual rooms.
* **`tiles/`** — Contains custom tile mappings, tags, textures, and collision properties (`is_solid`).

---

## How to Use This Template

1. **Clone or Copy:** Copy the `example` folder inside your local `user://packs/` directory (or use the in-game Pack Editor to create a new pack from scratch).
2. **Modify & Customize:** Update the `manifest.json` with your own unique namespace, author name, and description. Add your custom JSON files into the respective subdirectories.
3. **Test In-Game:** Launch *Hollow Descent*, open the **Pack Manager**, ensure your pack is enabled, and test your rooms and tiles directly in a run!