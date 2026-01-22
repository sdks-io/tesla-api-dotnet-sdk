
# Charging Location

*This model accepts additional fields of type object.*

## Structure

`ChargingLocation`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Name` | `string` | Optional | - |
| `Type` | `string` | Optional | - |
| `DistanceMiles` | `double?` | Optional | - |
| `Amenities` | `string` | Optional | - |
| `AvailableStalls` | `int?` | Optional | - |
| `TotalStalls` | `int?` | Optional | - |
| `SiteClosed` | `bool?` | Optional | - |
| `BillingInfo` | `string` | Optional | - |
| `Location` | [`Location1`](../../doc/models/location-1.md) | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "name": "name0",
  "type": "type0",
  "distance_miles": 123.84,
  "amenities": "amenities0",
  "available_stalls": 60,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

