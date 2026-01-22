
# Response 2

*This model accepts additional fields of type object.*

## Structure

`Response2`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Signaling` | [`Signaling`](../../doc/models/signaling.md) | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "signaling": {
    "enabled": false,
    "subscribe_connectivity": false,
    "use_auth_token": false,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

