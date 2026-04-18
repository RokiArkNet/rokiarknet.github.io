# DinoLoot v2.1

Add configurable loot drops to wild dino corpses on death. Perfect for custom progression and resource farming.

## Features

- **Pattern-Based Matching** - Match dinos by partial blueprint name (e.g., `Alpha_` matches all alphas)
- **Loot Pools** - Define multiple pools per dino with separate drop counts
- **Random Quantities** - Set MinQuantity/MaxQuantity for randomized item amounts
- **Quality Ranges** - Set MinQuality/MaxQuality for randomized item quality
- **Blueprint Drops** - Configurable chance to drop as blueprint instead of item
- **Harvest Multiplier** - Optional per-pool scaling based on server's harvest rate
- **Player Notification** - Optional chat message when loot is acquired
- **Tamed Excluded** - Only wild dino kills trigger loot drops

## Free Mode Limitations

Without a license, DinoLoot runs in free mode:
- **2 dino definitions maximum** (first 2 in config)
- Full features available, just limited count

## Configuration Preview

```json
{
  "Settings": {
    "ChatPrefix": "DinoLoot",
    "MessageOnDrop": true
  },
  "DinoLoot": {
    "Alpha_Character_BP": {
      "Pools": [
        {
          "Name": "Resources",
          "DropCount": 5,
          "UseHarvestMultiplier": true,
          "Items": [
            {
              "Blueprint": "Blueprint'/Game/.../PrimalItemResource_Hide'",
              "MinQuantity": 50,
              "MaxQuantity": 100
            }
          ]
        },
        {
          "Name": "Armor",
          "DropCount": 1,
          "Items": [
            {
              "Blueprint": "Blueprint'/Game/.../PrimalItemArmor_Saddle'",
              "Quantity": 1,
              "MinQuality": 1.0,
              "MaxQuality": 6.0,
              "BlueprintChance": 0.5
            }
          ]
        }
      ]
    }
  },
  "LicenseKey": "YOUR-LICENSE-KEY"
}
```

### Item Fields

| Field | Description |
|-------|-------------|
| `Blueprint` | Full blueprint path to the item |
| `MinQuantity` | Minimum quantity to drop |
| `MaxQuantity` | Maximum quantity to drop |
| `MinQuality` | Minimum item quality (1.0 = primitive) |
| `MaxQuality` | Maximum item quality |
| `BlueprintChance` | Chance (0.0-1.0) to drop as blueprint |

### Pool Fields

| Field | Description |
|-------|-------------|
| `Name` | Pool name (for logging) |
| `DropCount` | Number of items to randomly select |
| `UseHarvestMultiplier` | Scale quantities by server harvest rate |
| `Items` | Array of possible items in this pool |

## Console Commands

| Command | Description |
|---------|-------------|
| `DinoLoot.Reload` | Reload configuration (admin only) |
| `DinoLoot.List` | Show loaded dino definitions (admin only) |

---

## How to Purchase

### Step 1: Purchase License
Visit: **https://ko-fi.com/s/84cee00e04**

### Step 2: Join Discord
Join our Discord server: **https://discord.gg/qsbhxDEUfw**

### Step 3: Claim Your License
1. Go to the `#license-claims` channel
2. Use the `/claim` command with your Ko-fi email
3. You will receive your license key and the full plugin download

### Step 4: Install
1. Extract to `ArkApi/Plugins/DinoLoot/`
2. Add your license key to `config.json`
3. Restart server or use `DinoLoot.Reload`

---

## License Details

| Feature | Details |
|---------|---------|
| **Duration** | Annual license (365 days) |
| **Binding** | Per-machine (hardware ID) |
| **Servers** | Unlimited servers on same machine |
| **Transfers** | 3 transfers to new hardware included |

---

## Support

- **Discord**: https://discord.gg/qsbhxDEUfw
- **Ko-fi**: https://ko-fi.com/rokiarknet

## Version History

- **v2.1** - Per-pool harvest multiplier support
- **v2.0** - Quantity ranges, quality ranges, freemium licensing
- **v1.0** - Initial release
