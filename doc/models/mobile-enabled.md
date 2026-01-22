
# Mobile Enabled

*This model accepts additional fields of type object.*

## Structure

`MobileEnabled`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Result` | `bool?` | Optional | - |
| `Reason` | `string` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "result": false,
  "reason": "reason2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

