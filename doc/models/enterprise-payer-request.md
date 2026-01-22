
# Enterprise Payer Request

*This model accepts additional fields of type object.*

## Structure

`EnterprisePayerRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Role` | `string` | Required | - |
| `FederationId` | `string` | Optional | - |
| `AccountId` | `string` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "role": "role0",
  "federation_id": "federation_id0",
  "account_id": "account_id8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

