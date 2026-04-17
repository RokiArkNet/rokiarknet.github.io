# RiderProtection

Protect mounted players from taking damage.

## Features

- **Damage Reduction** - Reduce or eliminate damage to mounted players
- **Configurable Protection** - Set protection percentage per dino type
- **PvE/PvP Options** - Different settings for different scenarios

## Commands

| Command | Description |
|---------|-------------|
| `RiderProtection.Reload` | Reload configuration |

## Configuration

```json
{
  "Settings": {
    "Enabled": true,
    "DefaultProtection": 0.5
  },
  "Overrides": {
    "Rex_Character_BP": 1.0,
    "Giga_Character_BP": 0.75
  }
}
```

### Settings

- `DefaultProtection` - Default damage reduction (0.0 = none, 1.0 = full)
- `Overrides` - Per-dino protection values

## License

**Free** - No license required.
