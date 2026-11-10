# SHADOW SYSTEM ∞: The Eternal Monarch

A standalone, choice-driven dark-fantasy browser RPG. Create an awakener, explore the Ashen Frontier, descend into scaling gates, defeat enemies, build a shadow legion, and develop your character across an endless level curve.

## Run locally

The game uses plain HTML, CSS, and JavaScript—there is no build step or package install.

1. Start a static web server in this folder, for example:
   ```sh
   python3 -m http.server 8000
   ```
2. Open <http://localhost:8000> in a modern browser.

You can also open `index.html` directly, though some browser privacy settings may limit local saves when using a `file://` URL. Progress is stored in this browser’s `localStorage`; clearing browser data removes the save. There is no account, server-side save, external AI game master, or gameplay API integration. Custom actions use local keyword-based interpretation and procedural variations.

## Gameplay

- Create a character and select one of three origins.
- Explore the frontier, inspect gate runes, rest, and enter procedurally varied dungeon chambers.
- Fight level-scaled enemies, allocate attribute points, unlock techniques, and evolve your class at level 10.
- Attempt to extract defeated enemies as shadows, accept side directives, join a guild, and use supplies from your inventory.
- Use the System Admin panel for local testing tools. Reset deletes this game’s local save.
- On narrow screens the interface adapts for mobile; the desktop navigation sidebar is hidden on small screens.

The `start.sh` and `capture.sh` files are harness-specific helpers that expect an injected `RUNTIME_DIR`; they are not required for local play.

## Project files

- `index.html` — screen structure and controls
- `style.css` — responsive visual design
- `game.js` — game state, procedural encounters, UI, and local saves
