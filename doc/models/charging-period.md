
# Charging Period

*This model accepts additional fields of type object.*

## Structure

`ChargingPeriod`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `StartDateTime` | `string` | Optional | - |
| `Dimensions` | [`List<ChargingDimension>`](../../doc/models/charging-dimension.md) | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "start_date_time": "start_date_time8",
  "dimensions": [
    {
      "type": "type6",
      "volume": 148.9,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "type": "type6",
      "volume": 148.9,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

