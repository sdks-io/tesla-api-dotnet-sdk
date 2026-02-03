
# Adjust Volume Request

*This model accepts additional fields of type object.*

## Structure

`AdjustVolumeRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Volume` | `int` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "volume": 110,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

