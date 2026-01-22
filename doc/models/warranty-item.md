
# Warranty Item

*This model accepts additional fields of type object.*

## Structure

`WarrantyItem`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `WarrantyType` | `string` | Optional | - |
| `WarrantyDisplayName` | `string` | Optional | - |
| `ExpirationDate` | `DateTime?` | Optional | - |
| `ExpirationOdometer` | `int?` | Optional | - |
| `OdometerUnit` | `string` | Optional | - |
| `WarrantyExpiredOn` | `string` | Optional | - |
| `CoverageAgeInYears` | `int?` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "warrantyType": "warrantyType8",
  "warrantyDisplayName": "warrantyDisplayName0",
  "expirationDate": "2016-03-13T12:52:32.123Z",
  "expirationOdometer": 224,
  "odometerUnit": "odometerUnit6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

