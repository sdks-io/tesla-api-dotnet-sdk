
# Register Partner Response

*This model accepts additional fields of type object.*

## Structure

`RegisterPartnerResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Response` | [`ResponseRegisterPartnerResponse`](../../doc/models/response-register-partner-response.md) | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "response": {
    "client_id": "client_id2",
    "name": "name0",
    "description": "description0",
    "domain": "domain6",
    "ca": "ca4",
    "created_at": "2016-03-13T12:52:32.123Z",
    "updated_at": "2016-03-13T12:52:32.123Z",
    "enterprise_tier": "enterprise_tier6",
    "account_id": "account_id2",
    "issuer": "issuer0",
    "csr": "csr0",
    "csr_updated_at": "2016-03-13T12:52:32.123Z",
    "public_key": "public_key6",
    "public_key_hash": "public_key_hash8",
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

