
# Me Response

*This model accepts additional fields of type object.*

## Structure

`MeResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Response` | [`ResponseMeResponse`](../../doc/models/response-me-response.md) | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "response": {
    "email": "email6",
    "full_name": "full_name6",
    "profile_image_url": "profile_image_url6",
    "vault_uuid": "000012c4-0000-0000-0000-000000000000",
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

