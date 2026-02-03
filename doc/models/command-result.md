
# Command Result

*This model accepts additional fields of type object.*

## Structure

`CommandResult`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Result` | `bool` | Required | - |
| `Reason` | `string` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "result": false,
  "reason": "reason0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

