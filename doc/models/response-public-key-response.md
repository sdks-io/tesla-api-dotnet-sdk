
# Response Public Key Response

*This model accepts additional fields of type object.*

## Structure

`ResponsePublicKeyResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `PublicKey` | `string` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "public_key": "public_key0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

