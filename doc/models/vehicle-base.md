
# Vehicle Base

*This model accepts additional fields of type object.*

## Structure

`VehicleBase`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Id` | `int?` | Optional | - |
| `VehicleId` | `int?` | Optional | - |
| `Vin` | `string` | Optional | - |
| `DisplayName` | `string` | Optional | - |
| `AccessType` | `string` | Optional | - |
| `State` | `string` | Optional | - |
| `InService` | `bool?` | Optional | - |
| `CalendarEnabled` | `bool?` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "id": 126,
  "vehicle_id": 120,
  "vin": "vin8",
  "display_name": "display_name4",
  "access_type": "access_type0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

