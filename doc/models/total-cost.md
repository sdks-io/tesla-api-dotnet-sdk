
# Total Cost

*This model accepts additional fields of type object.*

## Structure

`TotalCost`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `ExclVat` | `double?` | Optional | - |
| `InclVat` | `double?` | Optional | - |
| `Vat` | `double?` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "excl_vat": 13.82,
  "incl_vat": 65.46,
  "vat": 170.96,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

