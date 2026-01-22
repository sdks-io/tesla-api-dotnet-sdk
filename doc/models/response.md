
# Response

*This model accepts additional fields of type object.*

## Structure

`Response`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Code` | `int` | Required | - |
| `Message` | `string` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "code": 46,
  "message": "message4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

