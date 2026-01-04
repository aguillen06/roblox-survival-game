# Survival Game - Promo Codes

## Active Codes

| Code | Coins | Bonus | Expiry |
|------|-------|-------|--------|
| LAUNCH | 100 | - | Never |
| SURVIVAL | 50 | - | Never |
| THANKYOU | 75 | - | Never |
| VIP100 | 100 | - | Never |
| COINS500 | 500 | - | Never |
| SPEEDBOOST | 25 | Speed Boost | Never |
| LUCKY | 150 | - | Never |
| YOUTUBE | 200 | - | Never |
| TWITTER | 100 | - | Never |
| DISCORD | 100 | - | Never |

## Adding New Codes

### In Roblox Studio

1. Open `ServerScriptService/CodesSystem`
2. Find the `ActiveCodes` table
3. Add new code:

```lua
ActiveCodes = {
    -- Existing codes...

    -- Add new code here:
    NEWCODE = {coins = 100, bonus = nil, expiry = nil},

    -- With expiry (expires in 7 days):
    LIMITED = {coins = 500, bonus = nil, expiry = os.time() + (7 * 24 * 60 * 60)},

    -- With bonus item:
    SPEEDCODE = {coins = 50, bonus = "boost_speed", expiry = nil},
}
```

### Bonus Types
- `boost_speed` - Temporary speed boost
- `boost_shield` - Temporary shield
- `nil` - No bonus, just coins

## Code Ideas for Marketing

### Social Media
- `FOLLOW` - Follow on Twitter/X reward
- `SUBSCRIBE` - YouTube subscriber reward
- `JOINUS` - Discord member reward

### Milestones
- `1KLIKES` - 1,000 likes celebration
- `10KVISITS` - 10K visits milestone
- `100KPLAYS` - 100K plays celebration

### Holidays
- `NEWYEAR2024` - New Year special
- `SUMMER2024` - Summer event
- `HALLOWEEN` - Halloween special
- `CHRISTMAS` - Christmas gift

### Influencer Codes
- `[YOUTUBER]` - YouTuber's custom code
- `[STREAMER]` - Streamer's custom code

### Limited Time
- `FLASH100` - Flash sale (24 hours)
- `WEEKEND` - Weekend special
- `MONDAY` - Monday motivation

## Tracking Code Usage

Codes are tracked per-player in DataStore. To see usage stats, you'd need to implement analytics or use Roblox's built-in analytics dashboard.

## Expired Codes Archive

| Code | Was | Expired |
|------|-----|---------|
| (none yet) | - | - |

---

*Update this file whenever you add or expire codes for your records.*
