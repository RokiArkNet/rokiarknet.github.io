# EngramControl

Block engrams from being learned, and unlock them by killing specific creatures.

## Features

- **Block Engrams** - Prevent players from learning specified engrams
- **Kill Unlocks** - Unlock engrams by killing bosses or creatures
- **Persistent Unlocks** - Player unlocks survive mindwipes
- **Pattern Matching** - Use partial names to match multiple engrams/creatures
- **License Validation** - Freemium model (5 engrams free, unlimited with license)

## Commands

| Command | Description |
|---------|-------------|
| `EngramControl.Reload` | Reload configuration |
| `EngramControl.Find <pattern>` | Search for engram names |

## Configuration

```json
{
  "General": {
    "Debug": false,
    "LogBlocks": true,
    "LogUnlocks": true
  },
  "BlockedEngrams": [
    "EngramEntry_TekReplicator",
    "EngramEntry_TekGenerator",
    "EngramEntry_C4"
  ],
  "KillUnlocks": {
    "BossArena_Broodmother": [
      "EngramEntry_TekReplicator",
      "EngramEntry_TekBoots"
    ],
    "Alpha_Rex": [
      "EngramEntry_RexSaddle_Tek"
    ]
  },
  "LicenseKey": "YOUR-LICENSE-KEY"
}
```

### BlockedEngrams

Array of engram entry names to block. Use `EngramControl.Find` in-game to discover names.

Pattern matching is supported - `Tek` matches all engrams containing "Tek".

### KillUnlocks

Map of creature patterns to engram arrays. When a matching creature dies, nearby players unlock those engrams.

- `BossArena_` - Matches all boss arenas
- `Alpha_` - Matches all alpha creatures
- Specific names like `Rex_Character_BP_C`

## License

Annual license required for full features. Free mode limits:

- Maximum 5 blocked engrams
- Kill unlocks disabled
- No persistent player data

Purchase at [ko-fi.com/rokiarknet](https://ko-fi.com/rokiarknet)
