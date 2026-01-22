
# Signaling

*This model accepts additional fields of type object.*

## Structure

`Signaling`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Enabled` | `bool` | Required | - |
| `SubscribeConnectivity` | `bool` | Required | - |
| `UseAuthToken` | `bool` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "enabled": false,
  "subscribe_connectivity": false,
  "use_auth_token": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

