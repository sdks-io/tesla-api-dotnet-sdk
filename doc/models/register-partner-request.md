
# Register Partner Request

*This model accepts additional fields of type object.*

## Structure

`RegisterPartnerRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Domain` | `string` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "domain": "domain.com",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

