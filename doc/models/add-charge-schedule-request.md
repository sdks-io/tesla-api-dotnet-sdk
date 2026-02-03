
# Add Charge Schedule Request

*This model accepts additional fields of type object.*

## Structure

`AddChargeScheduleRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Lat` | `double` | Required | - |
| `Lon` | `double` | Required | - |
| `Id` | `int` | Required | - |
| `DaysOfWeek` | `string` | Optional | - |
| `StartEnabled` | `bool?` | Optional | - |
| `StartTime` | `int?` | Optional | - |
| `EndEnabled` | `bool?` | Optional | - |
| `EndTime` | `int?` | Optional | - |
| `OneTime` | `bool?` | Optional | - |
| `Enabled` | `bool` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "lat": 196.62,
  "lon": 29.72,
  "id": 190,
  "days_of_week": "days_of_week8",
  "start_enabled": false,
  "start_time": 214,
  "end_enabled": false,
  "end_time": 174,
  "enabled": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

