
# Time of Use Settings Request

*This model accepts additional fields of type object.*

## Structure

`TimeOfUseSettingsRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `TouSettings` | [`TouSettings`](../../doc/models/tou-settings.md) | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "tou_settings": {
    "tariff_content_v2": {
      "key1": "val1",
      "key2": "val2"
    },
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

