
# Price Component

*This model accepts additional fields of type object.*

## Structure

`PriceComponent`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Type` | `string` | Optional | - |
| `Price` | `double?` | Optional | - |
| `StepSize` | `double?` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "type": "type2",
  "price": 87.54,
  "step_size": 214.68,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

