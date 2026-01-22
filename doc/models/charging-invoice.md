
# Charging Invoice

*This model accepts additional fields of type object.*

## Structure

`ChargingInvoice`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `FileName` | `string` | Optional | - |
| `ContentId` | `string` | Optional | - |
| `InvoiceType` | `string` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "fileName": "fileName0",
  "contentId": "contentId0",
  "invoiceType": "invoiceType0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

