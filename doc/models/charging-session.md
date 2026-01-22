
# Charging Session

*This model accepts additional fields of type object.*

## Structure

`ChargingSession`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Id` | `string` | Optional | - |
| `Vin` | `string` | Optional | - |
| `Model` | `string` | Optional | - |
| `StartDateTime` | `string` | Optional | - |
| `StopDateTime` | `string` | Optional | - |
| `TotalEnergy` | `double?` | Optional | - |
| `TotalTime` | `double?` | Optional | - |
| `TotalCost` | [`TotalCost`](../../doc/models/total-cost.md) | Optional | - |
| `Location` | [`Location`](../../doc/models/location.md) | Optional | - |
| `ChargingPeriods` | [`List<ChargingPeriod>`](../../doc/models/charging-period.md) | Optional | - |
| `Tariffs` | [`Tariffs`](../../doc/models/tariffs.md) | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "id": "id0",
  "vin": "vin6",
  "model": "model8",
  "start_date_time": "start_date_time6",
  "stop_date_time": "stop_date_time2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

