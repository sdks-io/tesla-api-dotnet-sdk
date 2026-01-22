
# Public Key Response

*This model accepts additional fields of type object.*

## Structure

`PublicKeyResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Response` | [`ResponsePublicKeyResponse`](../../doc/models/response-public-key-response.md) | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "response": {
    "public_key": "public_key6",
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

