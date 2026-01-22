
# Operation Request

*This model accepts additional fields of type object.*

## Structure

`OperationRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `DefaultRealMode` | [`DefaultRealMode`](../../doc/models/default-real-mode.md) | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "default_real_mode": "autonomous",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

