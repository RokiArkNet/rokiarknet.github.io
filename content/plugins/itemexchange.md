# ItemExchange

Exchange items between players with configurable rates.

## Features

- **Item Trading** - Exchange items at configured ratios
- **Currency Support** - Use any item as currency
- **Admin Controls** - Configure exchange rates

## Commands

| Command | Description |
|---------|-------------|
| `ItemExchange.Reload` | Reload configuration |

## Configuration

```json
{
  "Settings": {
    "Enabled": true,
    "ChatPrefix": "Exchange"
  },
  "Exchanges": {
    "MetalToElement": {
      "Input": "PrimalItemResource_Metal",
      "InputAmount": 1000,
      "Output": "PrimalItemResource_Element",
      "OutputAmount": 1
    }
  }
}
```

## License

**Free** - No license required.
