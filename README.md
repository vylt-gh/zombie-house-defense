# Zombie House Defense

Top-down zombie survival game with procedurally generated rooms, permanent upgrades, and a roguelike loop.

## Play

Open `game.html` in a browser. No server needed.

## Controls

| Key | Action |
|-----|--------|
| WASD / Arrows | Move |
| Hold left click | Aim & fire |
| E | Interact (unlock doors, buy upgrades, eat food) |
| R | Restart after death |
| " | Toggle debug panel |

### Debug cheats (after pressing ")

| Key | Effect |
|-----|--------|
| 1 | Noclip |
| 2 | 2x speed |
| 3 | God mode |
| 4 | Grant all upgrades |
| 5 | +100 coins |
| 6 | Heal to full |
| 7 | Spawn 5 zombies |

## Gameplay

- Fight through infinite linear rooms. Each room costs coins to unlock.
- Zombies get harder over time (speed, damage, spawn rate).
- Three zombie types: regular (60%), fast (20%), big (20%).
- Kill zombies for coins. Coins auto-attract within range.
- Life steal: each bullet hit heals 0.5 HP.

## Room Effects

| Room | Effect |
|------|--------|
| Armory | Buy dual-shot + fire rate upgrade (100 coins) |
| Forge | Buy sword — auto-slash melee (50 coins) |
| Workshop | Buy +1 bullet damage (100 coins) |
| Treasury | +1 coin per kill (guaranteed) |
| Library | 20% more coins from all sources |
| Infirmary | +30 HP on entry |
| Kitchen / Dining Hall / Pantry | Food items — eat for 5 HP each |
| Sanctuary / Spa | Slow passive HP regen while inside |
| Shooting Range | Permanent fire rate boost (0.7x) |
| Enchanting Table | Bullets pierce zombies |
| Gate Room | Bullets knock zombies back |
| Observatory | +5° aim assist arc |
| Dungeon | Extra zombies spawn while inside |

## Upgrades

Upgrades stack. Fire rate is multiplicative (base 0.35s). Armory and Shooting Range both reduce it.

## Tech

Single HTML file (~1500 lines). Canvas 2D rendering. Web Audio API for sound effects. No dependencies.
