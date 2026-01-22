
# Charging Sessions Response

*This model accepts additional fields of type object.*

## Structure

`ChargingSessionsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Response` | [`ChargingSessionsData`](../../doc/models/charging-sessions-data.md) | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "response": {
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
    "status_code": 216,
    "status_message": "status_message8",
    "timestamp": {
      "key0": "timestamp1",
      "key1": "timestamp2",
      "key2": "timestamp3"
    },
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

