# EngramControl v5.0

Block engrams globally and unlock them through gameplay. Perfect for progression servers with boss-based unlocks.

## Features

- **Block Engrams** - Prevent players from learning specific engrams using exact names or partial matching
- **KillUnlocks** - Unblock engrams after killing specific creatures (player must still learn them)
- **GrantUnlocks** - Directly teach engrams when creatures are killed (auto-learned, no crafting required)
- **Variable Unlock Count** - Randomly grant N engrams from a pool (minUnlock/maxUnlock)
- **Smart Filtering** - Only grants engrams the player doesn't already have
- **Radius-Based Rewards** - All players near the kill receive the unlock
- **Persistent Unlocks** - Player unlocks survive mindwipes and server restarts
- **Admin Commands** - Search engrams and reload config without restart

## Free Mode Limitations

Without a license, EngramControl runs in free mode:
- **5 blocked engrams maximum**
- Full features available, just limited count

## Configuration Preview

```json
{
  "BlockedEngrams": ["Alpha", "Demonic", "Tek"],
  "KillUnlocks": {
    "Boss Progression": {
      "engrams": ["Alpha", "Kibble_Alpha"],
      "required_kills": ["AlphaBoss_Character_BP"]
    }
  },
  "GrantUnlocks": {
    "Broodmother_Character_BP": {
      "engrams": [
        "Blueprint'/Game/.../PrimalItemStructure_TekReplicator'",
        "Blueprint'/Game/.../PrimalItemStructure_TekGenerator'"
      ],
      "minUnlock": 1,
      "maxUnlock": 2
    }
  },
  "LicenseKey": "YOUR-LICENSE-KEY"
}
```

## Console Commands

| Command | Description |
|---------|-------------|
| `EngramControl.Reload` | Reload config and player unlocks |
| `EngramControl.Find <pattern>` | Search engrams (shows mod source) |
| `EngramControl.Progress` | Show player's kill progress |

---

## How to Purchase

### Step 1: Purchase License
Visit: **https://ko-fi.com/s/af98e82d0e**

### Step 2: Join Discord
Join our Discord server: **https://discord.gg/qsbhxDEUfw**

### Step 3: Claim Your License
1. Go to the `#license-claims` channel
2. Use the `/claim` command with your Ko-fi email
3. You will receive your license key and the full plugin download

### Step 4: Install
1. Extract to `ArkApi/Plugins/EngramControl/`
2. Add your license key to `config.json`
3. Restart server or use `EngramControl.Reload`

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

- **v5.0** - Added GrantUnlocks (direct teaching), variable unlock count
- **v4.0** - Multi-kill requirements, improved progress tracking
- **v3.5** - HWID licensing, mod source display
