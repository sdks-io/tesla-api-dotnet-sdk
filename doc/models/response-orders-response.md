
# Response Orders Response

*This model accepts additional fields of type object.*

## Structure

`ResponseOrdersResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `VehicleMapId` | `int` | Required | - |
| `ReferenceNumber` | `string` | Required | - |
| `Vin` | `string` | Required | - |
| `OrderStatus` | `string` | Required | - |
| `OrderSubstatus` | `string` | Required | - |
| `ModelCode` | `string` | Required | - |
| `CountryCode` | `string` | Required | - |
| `Locale` | `string` | Required | - |
| `MktOptions` | `string` | Required | - |
| `IsB2B` | `bool` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "vehicleMapId": 198,
  "referenceNumber": "referenceNumber2",
  "vin": "vin8",
  "orderStatus": "orderStatus6",
  "orderSubstatus": "orderSubstatus2",
  "modelCode": "modelCode6",
  "countryCode": "countryCode6",
  "locale": "locale6",
  "mktOptions": "mktOptions2",
  "isB2b": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

