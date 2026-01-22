
# Response Register Partner Response

*This model accepts additional fields of type object.*

## Structure

`ResponseRegisterPartnerResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `ClientId` | `string` | Required | - |
| `Name` | `string` | Required | - |
| `Description` | `string` | Optional | - |
| `Domain` | `string` | Required | - |
| `Ca` | `string` | Optional | - |
| `CreatedAt` | `DateTime` | Required | - |
| `UpdatedAt` | `DateTime` | Required | - |
| `EnterpriseTier` | `string` | Required | - |
| `AccountId` | `string` | Required | - |
| `Issuer` | `string` | Optional | - |
| `Csr` | `string` | Optional | - |
| `CsrUpdatedAt` | `DateTime?` | Optional | - |
| `PublicKey` | `string` | Required | - |
| `PublicKeyHash` | `string` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "client_id": "client_id6",
  "name": "name4",
  "description": "description4",
  "domain": "domain0",
  "ca": "ca8",
  "created_at": "2016-03-13T12:52:32.123Z",
  "updated_at": "2016-03-13T12:52:32.123Z",
  "enterprise_tier": "enterprise_tier8",
  "account_id": "account_id6",
  "issuer": "issuer4",
  "csr": "csr6",
  "csr_updated_at": "2016-03-13T12:52:32.123Z",
  "public_key": "public_key2",
  "public_key_hash": "public_key_hash2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

