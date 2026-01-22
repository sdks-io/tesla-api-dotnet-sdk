
# Charge Start Time

*This model accepts additional fields of type object.*

## Structure

`ChargeStartTime`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Seconds` | `int` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "seconds": 90,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

