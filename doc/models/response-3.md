
# Response 3

*This model accepts additional fields of type object.*

## Structure

`Response3`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `DestinationCharging` | [`List<ChargingLocation>`](../../doc/models/charging-location.md) | Optional | - |
| `Superchargers` | [`List<ChargingLocation>`](../../doc/models/charging-location.md) | Optional | - |
| `Timestamp` | `int?` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "destination_charging": [
    {
      "name": "name8",
      "type": "type2",
      "distance_miles": 106.72,
      "amenities": "amenities8",
      "available_stalls": 140,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "name": "name8",
      "type": "type2",
      "distance_miles": 106.72,
      "amenities": "amenities8",
      "available_stalls": 140,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "name": "name8",
      "type": "type2",
      "distance_miles": 106.72,
      "amenities": "amenities8",
      "available_stalls": 140,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "superchargers": [
    {
      "name": "name0",
      "type": "type0",
      "distance_miles": 190.44,
      "amenities": "amenities0",
      "available_stalls": 64,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "timestamp": 194,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

