
# Response Me Response

*This model accepts additional fields of type object.*

## Structure

`ResponseMeResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Email` | `string` | Required | - |
| `FullName` | `string` | Required | - |
| `ProfileImageUrl` | `string` | Required | - |
| `VaultUuid` | `Guid` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "email": "email4",
  "full_name": "full_name8",
  "profile_image_url": "profile_image_url8",
  "vault_uuid": "000013ee-0000-0000-0000-000000000000",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

