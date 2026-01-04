# Game Pass IDs

After creating game passes on Roblox, record their IDs here and update `ServerScriptService/GamePassSystem`.

## Pass IDs (Fill in after creating)

| Pass Name | Price | Roblox Pass ID |
|-----------|-------|----------------|
| VIP Pass | R$ 399 | `__________` |
| Double Coins | R$ 149 | `__________` |
| Speed Demon | R$ 99 | `__________` |
| Tank | R$ 149 | `__________` |
| Lucky Charm | R$ 199 | `__________` |
| DJ Pass | R$ 249 | `__________` |

## How to Get Pass ID

1. Go to Roblox Creator Dashboard
2. Select your game
3. Go to Monetization > Game Passes
4. Create each pass with icon and description
5. Copy the numeric ID from the URL or pass details

## Update GamePassSystem Script

```lua
local GamePasses = {
    VIP = {
        id = 123456789, -- Replace with actual ID
        name = "VIP Pass",
        price = 399,
        -- ...
    },
    DoubleCoins = {
        id = 123456790, -- Replace with actual ID
        name = "Double Coins",
        price = 149,
        -- ...
    },
    -- etc.
}
```

## Pass Descriptions for Roblox

### VIP Pass (R$ 399)
**Title:** VIP Pass
**Description:** The ultimate survival package! Get 2x coins on everything, an exclusive VIP chat tag, and a stunning golden trail. Show everyone you're a true survivor!

### Double Coins (R$ 149)
**Title:** Double Coins
**Description:** Double your coin earnings forever! Every second you survive, every achievement you unlock - 2x the coins!

### Speed Demon (R$ 99)
**Title:** Speed Demon
**Description:** Move 25% faster permanently! Dodge hazards easier, collect food faster, and outrun those pesky enemies.

### Tank (R$ 149)
**Title:** Tank
**Description:** Start every game with 150 HP instead of 100. More health means more survival time and more coins!

### Lucky Charm (R$ 199)
**Title:** Lucky Charm
**Description:** Food spawns closer to you, and power-ups last 50% longer! Lady Luck is on your side.

### DJ Pass (R$ 249)
**Title:** DJ Pass
**Description:** Take control of the music! Play your favorite Roblox audio for everyone in the server. Be the life of the party!

---

*Remember to create eye-catching icons for each pass!*
