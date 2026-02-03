
# Guest Mode Request

*This model accepts additional fields of type object.*

## Structure

`GuestModeRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Enable` | `bool` | Required | Enable or disable Guest Mode |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "enable": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

