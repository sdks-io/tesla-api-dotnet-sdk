
# Pagination

*This model accepts additional fields of type object.*

## Structure

`Pagination`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Previous` | `int?` | Optional | - |
| `Next` | `int?` | Optional | - |
| `Current` | `int?` | Optional | - |
| `PerPage` | `int?` | Optional | - |
| `Count` | `int?` | Optional | - |
| `Pages` | `int?` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "previous": 176,
  "next": 10,
  "current": 16,
  "per_page": 92,
  "count": 210,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

