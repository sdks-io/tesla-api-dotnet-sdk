
# Charging Dimension

*This model accepts additional fields of type object.*

## Structure

`ChargingDimension`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Type` | `string` | Optional | - |
| `Volume` | `double?` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "type": "type0",
  "volume": 253.86,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

