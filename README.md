# Survival Game - Roblox

A complete survival game built with Claude Code and Roblox Studio MCP.

## Game Overview

Players must survive as long as possible while avoiding hazards, collecting food, and earning coins. Features include a lobby system, shop, achievements, daily rewards, and more.

## Features

### Core Gameplay
- Health drain survival mechanic
- Food pickups for healing
- Multiple hazard types (fire, lava, acid, spikes)
- Moving obstacles (walls, crushers)
- Power-ups (speed, shield, heal, invincible)
- Moving hazards (fireballs, chasers, spinning blade)

### Progression Systems
- Coin currency from survival time
- 22 Achievements with rewards
- 7-day Daily Rewards cycle
- Leaderboard with DataStore persistence

### Lobby & UI
- Elevated lobby area at Y=100
- Play button to start game
- Shop, Achievements, Daily Rewards panels
- Difficulty selector (Easy, Normal, Hard, Extreme)
- Game Passes and Codes buttons

### Monetization
- **Private Servers**: 150 Robux
- **Game Passes**: 6 passes (R$99 - R$399)
- **Shop**: In-game coin purchases

### Quality of Life
- Tutorial for new players (7 steps)
- Mobile touch controls (joystick + jump)
- Codes system for promotions
- Music and sound effects (14 sounds)

## Game Passes

| Pass | Price | Perks |
|------|-------|-------|
| VIP Pass | R$ 399 | 2x Coins, VIP tag, Gold trail |
| Double Coins | R$ 149 | 2x coin earnings |
| Speed Demon | R$ 99 | +25% walk speed |
| Tank | R$ 149 | 150 HP (vs 100) |
| Lucky Charm | R$ 199 | Food magnet, +50% power-up duration |
| DJ Pass | R$ 249 | Play music for everyone |

## Setup Instructions

### 1. Publish Game
1. Open Roblox Studio with the project
2. File > Publish to Roblox
3. Configure game settings (name, description, icon)

### 2. Enable Private Servers
1. Game Settings > Monetization
2. Enable Private Servers
3. Set price to 150 Robux

### 3. Create Game Passes
1. Game Settings > Monetization > Game Passes
2. Create each pass with prices listed above
3. Copy Pass IDs into `ServerScriptService/GamePassSystem`

### 4. Configure Sounds
Upload these sound IDs to `ReplicatedStorage/GameSounds`:
- LobbyMusic, GameMusic
- FoodPickup, PowerUpPickup
- Damage, GameOver
- ButtonClick, Purchase
- Achievement, LevelUp
- Countdown, Victory, Defeat
- Heartbeat, Whoosh

## Active Codes

| Code | Reward |
|------|--------|
| LAUNCH | 100 coins |
| SURVIVAL | 50 coins |
| THANKYOU | 75 coins |
| VIP100 | 100 coins |
| COINS500 | 500 coins |
| SPEEDBOOST | 25 coins + speed boost |
| LUCKY | 150 coins |
| YOUTUBE | 200 coins |
| TWITTER | 100 coins |
| DISCORD | 100 coins |

### Adding New Codes
Edit `ServerScriptService/CodesSystem` and add to the `ActiveCodes` table:
```lua
NEWCODE = {coins = 100, bonus = nil, expiry = nil},
```

## Scripts Reference

### ServerScriptService
- `HealthSystem` - Health drain and game over
- `FoodSpawner` - Healing orb spawning
- `HazardSystem` - Static fire hazards
- `MovingObstacles` - Walls and crushers
- `PowerUpsSystem` - Buff pickups
- `MovingHazards` - Fireballs, chasers, blade
- `GameStateManager` - Lobby/game transitions
- `LeaderboardSystem` - Top scores
- `SoundManager` - Audio triggers
- `ShopSystem` - Currency and purchases
- `TrailSystem` - Player trails
- `DifficultySystem` - Difficulty scaling
- `AchievementSystem` - 22 achievements
- `DailyRewardsSystem` - 7-day rewards
- `PrivateServerSystem` - VIP server features
- `GamePassSystem` - Game pass perks
- `TutorialSystem` - New player tutorial
- `CodesSystem` - Promo codes

### StarterGui
- `SurvivalUI` - In-game HUD
- `LobbyUI` - Lobby interface
- `AchievementUI` - Unlock notifications
- `DailyRewardsUI` - Daily rewards popup
- `PrivateServerUI` - VIP controls
- `GamePassUI` - Pass shop
- `TutorialUI` - Tutorial screens
- `CodesUI` - Code redemption
- `MobileControlsUI` - Touch controls

## Difficulty Levels

| Level | Health Drain | Damage | Enemy Speed | Food Heal | Coin Multiplier |
|-------|-------------|--------|-------------|-----------|-----------------|
| Easy | 1 HP/sec | 0.5x | 0.75x | 35 HP | 0.75x |
| Normal | 2 HP/sec | 1x | 1x | 25 HP | 1x |
| Hard | 3 HP/sec | 1.5x | 1.25x | 20 HP | 1.5x |
| Extreme | 5 HP/sec | 2x | 1.5x | 15 HP | 2.5x |

## Credits

Built with Claude Code (Anthropic) using Roblox Studio MCP integration.
