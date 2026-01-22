
# Charging Fee

*This model accepts additional fields of type object.*

## Structure

`ChargingFee`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `SessionFeeId` | `int?` | Optional | - |
| `FeeType` | `string` | Optional | - |
| `CurrencyCode` | `string` | Optional | - |
| `PricingType` | `string` | Optional | - |
| `RateBase` | `double?` | Optional | - |
| `RateTier1` | `double?` | Optional | - |
| `RateTier2` | `double?` | Optional | - |
| `RateTier3` | `double?` | Optional | - |
| `RateTier4` | `double?` | Optional | - |
| `UsageBase` | `double?` | Optional | - |
| `UsageTier1` | `double?` | Optional | - |
| `UsageTier2` | `double?` | Optional | - |
| `UsageTier3` | `double?` | Optional | - |
| `UsageTier4` | `double?` | Optional | - |
| `TotalBase` | `double?` | Optional | - |
| `TotalTier1` | `double?` | Optional | - |
| `TotalTier2` | `double?` | Optional | - |
| `TotalTier3` | `double?` | Optional | - |
| `TotalTier4` | `double?` | Optional | - |
| `TotalDue` | `double?` | Optional | - |
| `NetDue` | `double?` | Optional | - |
| `Uom` | `string` | Optional | - |
| `IsPaid` | `bool?` | Optional | - |
| `Status` | `string` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "sessionFeeId": 236,
  "feeType": "feeType4",
  "currencyCode": "currencyCode0",
  "pricingType": "pricingType6",
  "rateBase": 226.56,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

