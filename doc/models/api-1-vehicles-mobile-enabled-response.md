
# Api 1 Vehicles Mobile Enabled Response

*This model accepts additional fields of type object.*

## Structure

`Api1VehiclesMobileEnabledResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Response` | [`MobileEnabled`](../../doc/models/mobile-enabled.md) | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "response": {
    "result": false,
    "reason": "reason4",
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

