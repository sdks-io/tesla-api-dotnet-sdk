
# Driver

*This model accepts additional fields of type object.*

## Structure

`Driver`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `MyTeslaUniqueId` | `int?` | Optional | - |
| `UserId` | `int?` | Optional | - |
| `UserIdS` | `string` | Optional | - |
| `VaultUuid` | `string` | Optional | - |
| `DriverFirstName` | `string` | Optional | - |
| `DriverLastName` | `string` | Optional | - |
| `GranularAccess` | `object` | Optional | - |
| `ActivePubkeys` | `List<string>` | Optional | - |
| `PublicKey` | `string` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "my_tesla_unique_id": 40,
  "user_id": 64,
  "user_id_s": "user_id_s4",
  "vault_uuid": "vault_uuid0",
  "driver_first_name": "driver_first_name2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

