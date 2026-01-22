
# Charging Sessions Data

*This model accepts additional fields of type object.*

## Structure

`ChargingSessionsData`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Data` | [`List<ChargingSession>`](../../doc/models/charging-session.md) | Optional | - |
| `StatusCode` | `int?` | Optional | - |
| `StatusMessage` | `string` | Optional | - |
| `Timestamp` | `Dictionary<string, string>` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "data": [
    {
      "id": "id0",
      "vin": "vin4",
      "model": "model8",
      "start_date_time": "start_date_time6",
      "stop_date_time": "stop_date_time2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "id": "id0",
      "vin": "vin4",
      "model": "model8",
      "start_date_time": "start_date_time6",
      "stop_date_time": "stop_date_time2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "id": "id0",
      "vin": "vin4",
      "model": "model8",
      "start_date_time": "start_date_time6",
      "stop_date_time": "stop_date_time2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "status_code": 188,
  "status_message": "status_message8",
  "timestamp": {
    "key0": "timestamp7",
    "key1": "timestamp8"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

