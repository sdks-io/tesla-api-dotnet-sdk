
# Response Live Status Response

*This model accepts additional fields of type object.*

## Structure

`ResponseLiveStatusResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `SolarPower` | `double` | Required | - |
| `EnergyLeft` | `double` | Required | - |
| `TotalPackEnergy` | `double` | Required | - |
| `PercentageCharged` | `double` | Required | - |
| `BackupCapable` | `bool` | Required | - |
| `BatteryPower` | `double?` | Optional | - |
| `LoadPower` | `double?` | Optional | - |
| `GridStatus` | `string` | Optional | - |
| `GridPower` | `double?` | Optional | - |
| `IslandStatus` | `string` | Optional | - |
| `StormModeActive` | `bool?` | Optional | - |
| `Timestamp` | `DateTime?` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "solar_power": 108.14,
  "energy_left": 185.46,
  "total_pack_energy": 65.2,
  "percentage_charged": 141.22,
  "backup_capable": false,
  "battery_power": 211.48,
  "load_power": 248.74,
  "grid_status": "grid_status2",
  "grid_power": 38.0,
  "island_status": "island_status4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

