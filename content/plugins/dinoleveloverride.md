# DinoLevelOverride

Override wild dino level distributions for custom spawning.

## Features

- **Custom Level Ranges** - Set min/max levels for wild dinos
- **Per-Dino Settings** - Different ranges for different species
- **Weighted Distribution** - Control level distribution curves

## Commands

| Command | Description |
|---------|-------------|
| `DinoLevelOverride.Reload` | Reload configuration |

## Configuration

```json
{
  "Settings": {
    "Enabled": true,
    "DefaultMinLevel": 1,
    "DefaultMaxLevel": 150
  },
  "Overrides": {
    "Rex_Character_BP": {
      "MinLevel": 50,
      "MaxLevel": 300
    },
    "Alpha_": {
      "MinLevel": 150,
      "MaxLevel": 500
    }
  }
}
```

## License

**Free** - No license required.
