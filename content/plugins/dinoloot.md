# DinoLoot

Add configurable loot drops to dino corpses when killed.

## Features

- **Custom Loot Pools** - Define what items drop from each dino type
- **Quality Ranges** - Set min/max quality for item drops
- **Blueprint Chance** - Configure chance for items to drop as blueprints
- **Pattern Matching** - Use partial dino names to match multiple species
- **Player Inventory** - Loot goes directly to killer's inventory

## Commands

| Command | Description |
|---------|-------------|
| `DinoLoot.Reload` | Reload configuration |
| `DinoLoot.List` | List configured dino loot definitions |

## Configuration

```json
{
  "Settings": {
    "ChatPrefix": "DinoLoot",
    "MessageOnDrop": true
  },
  "DinoLoot": {
    "Rex_Character_BP": {
      "Pools": [
        {
          "Name": "RexLoot",
          "DropCount": 2,
          "Items": [
            {
              "Blueprint": "Blueprint'/Game/PrimalEarth/CoreBlueprints/Items/Armor/Saddles/PrimalItemArmor_RexSaddle'",
              "Quantity": 1,
              "MinQuality": 1.0,
              "MaxQuality": 3.0,
              "BlueprintChance": 0.1
            },
            {
              "Blueprint": "Blueprint'/Game/PrimalEarth/CoreBlueprints/Resources/PrimalItemResource_Hide'",
              "Quantity": 50,
              "MinQuality": 1.0,
              "MaxQuality": 1.0,
              "BlueprintChance": 0.0
            }
          ]
        }
      ]
    },
    "Alpha_": {
      "Pools": [
        {
          "Name": "AlphaLoot",
          "DropCount": 3,
          "Items": [
            {
              "Blueprint": "Blueprint'/Game/PrimalEarth/CoreBlueprints/Resources/PrimalItemResource_Element'",
              "Quantity": 5,
              "MinQuality": 1.0,
              "MaxQuality": 1.0,
              "BlueprintChance": 0.0
            }
          ]
        }
      ]
    }
  }
}
```

### Settings

- `ChatPrefix` - Prefix for chat messages
- `MessageOnDrop` - Show message when loot drops

### DinoLoot

Map of dino patterns to loot pools:

- `DropCount` - Number of items to drop from the pool
- `Items` - Array of possible items
  - `Blueprint` - Item blueprint path (auto-fixes missing `.AssetName` suffix)
  - `Quantity` - Stack size
  - `MinQuality` / `MaxQuality` - Quality range (1.0 = primitive, 6.0 = ascendant)
  - `BlueprintChance` - Chance to drop as blueprint (0.0 - 1.0)

## License

Annual license required.

Purchase at [ko-fi.com/rokiarknet](https://ko-fi.com/rokiarknet)
