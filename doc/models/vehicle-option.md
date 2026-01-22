
# Vehicle Option

*This model accepts additional fields of type object.*

## Structure

`VehicleOption`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Code` | `string` | Optional | - |
| `DisplayName` | `string` | Optional | - |
| `ColorCode` | `string` | Optional | - |
| `IsActive` | `bool?` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "code": "code2",
  "displayName": "displayName8",
  "colorCode": "colorCode4",
  "isActive": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

