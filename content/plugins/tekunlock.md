# TekUnlock

Unlock Tek engrams by killing specific creatures.

## Features

- **Kill-Based Unlocks** - Kill bosses/creatures to unlock Tek engrams
- **Radius Detection** - All players within range get the unlock
- **Chat Notifications** - Notify players when they unlock new engrams

## Commands

| Command | Description |
|---------|-------------|
| `TekUnlock.Reload` | Reload configuration |

## Configuration

```json
{
  "Settings": {
    "ChatPrefix": "TekUnlock",
    "UnlockRadius": 50000.0,
    "MessageOnUnlock": true
  },
  "KillUnlocks": {
    "BossArena_Broodmother": [
      "Blueprint'/Game/PrimalEarth/CoreBlueprints/Items/Structures/Misc/PrimalItemStructure_TekReplicator.PrimalItemStructure_TekReplicator'"
    ],
    "Bone_Jerboa_Character_BP_AlphaBoss": [
      "Blueprint'/Game/PrimalEarth/CoreBlueprints/Items/Structures/Misc/PrimalItemStructure_TekGenerator.PrimalItemStructure_TekGenerator'"
    ]
  }
}
```

### Settings

- `ChatPrefix` - Prefix for chat messages
- `UnlockRadius` - Distance from kill to receive unlock (UE units)
- `MessageOnUnlock` - Show message when engrams unlock

### KillUnlocks

Map of creature patterns to blueprint arrays. Use full blueprint paths.

## License

Annual license required.

Purchase at [ko-fi.com/rokiarknet](https://ko-fi.com/rokiarknet)
