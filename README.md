# Zombie House Defense

<hr>

> [!IMPORTANT]
> so uhhhh i kinda hit the free token limit for my model with this project...
> they said it was unlimited idk what happened.
> i somehow found the limit to opencode zen "unlimited"
> (it was around 1.5m tokens in 2 days btw)
>
> so im no longer updating this project.
> unless i get a really good and expensive ai sub
> then maybe.
> but i am a child,
> so prob not.

<hr>

## CREDIT TO [@bilisimyonelt-del](https://github.com/bilisimyonelt-del) FOR THE IDEA

Top-down zombie survival game with procedurally generated rooms, permanent upgrades, and a roguelike loop.

Play: https://gameguyonyt.github.io/ZombieHouseDefense

## Controls

| Input | Action |
|-------|--------|
| WASD / Arrows | Move |
| Hold left click / right half of screen | Aim & fire |
| E / Space / tap bottom-center of screen | Interact (unlock doors, buy upgrades, eat food) |
| R | Restart after death |
| " | Toggle debug panel |

### Mobile

- **Twin-stick mode (default)**: Left side → joystick moves, Right side → joystick aims. Stationary joysticks stay fixed at bottom corners; dynamic ones appear at your touch position.
- **Screen-wide mode**: Left quarter → movement joystick, anywhere else → aim at your finger.
- Interact button at bottom-center of screen.

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
- Rooms generate horizontally in landscape, vertically in portrait.
- Zombies get harder over time (speed, damage, spawn rate).
- Three zombie types: regular (60%), fast (20%), big (20%).
- Kill zombies for coins. Coins auto-attract within range.
- Life steal: each bullet hit heals 0.5 HP.
- 10° aim lock-on arc snaps bullets to nearest zombie.
- Wall sliding via separated X/Y collision.

## Room Effects

| Room | Effect |
|------|--------|
| Armory | Buy dual-shot upgrade (100 coins) |
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
| Throne Room | Boss fight! Kill the king zombie for a 30s laser weapon |
| Dungeon | Extra zombies spawn while inside |

## Upgrades

Upgrades stack. Fire rate is multiplicative (base 0.35s). Shooting Range reduces it.

## Settings (gear icon on main menu)

| Setting | Options | Notes |
|---------|---------|-------|
| Door unlock | Walk through / Interact | Walk through = auto-unlock on contact |
| Interact mode | Interact (E) / Auto pickup | Upgrades and food: auto-collect on contact or press E |
| Aim mode | Joystick / Screen-wide | Mobile only |
| Joystick style | Stationary / Dynamic | Stationary = fixed bottom corners; Dynamic = appears at touch |
| Joystick position | Low / High | Mobile only. Low = default; High = moves joysticks + interact button ~250px up |
| Casual mode | Off / On | Zombies 25% slower, difficulty 25% slower, fire rate 0.25s |
| Auto-fire | Off / On | Gun fires continuously without holding any button |

## Tech

Single HTML file (~1900 lines). Canvas 2D rendering. Web Audio API for sound effects. No dependencies.
