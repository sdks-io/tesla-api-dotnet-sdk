
# Charging History Item

*This model accepts additional fields of type object.*

## Structure

`ChargingHistoryItem`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `SessionId` | `int` | Required | - |
| `Vin` | `string` | Required | - |
| `SiteLocationName` | `string` | Optional | - |
| `ChargeStartDateTime` | `DateTime?` | Optional | - |
| `ChargeStopDateTime` | `DateTime?` | Optional | - |
| `UnlatchDateTime` | `DateTime?` | Optional | - |
| `CountryCode` | `string` | Optional | - |
| `Fees` | [`List<ChargingFee>`](../../doc/models/charging-fee.md) | Optional | - |
| `BillingType` | `string` | Optional | - |
| `Invoices` | [`List<ChargingInvoice>`](../../doc/models/charging-invoice.md) | Optional | - |
| `VehicleMakeType` | `string` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "sessionId": 16,
  "vin": "vin0",
  "siteLocationName": "siteLocationName8",
  "chargeStartDateTime": "2016-03-13T12:52:32.123Z",
  "chargeStopDateTime": "2016-03-13T12:52:32.123Z",
  "unlatchDateTime": "2016-03-13T12:52:32.123Z",
  "countryCode": "countryCode8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

