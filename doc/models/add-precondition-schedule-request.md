
# Add Precondition Schedule Request

*This model accepts additional fields of type object.*

## Structure

`AddPreconditionScheduleRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Lat` | `double` | Required | - |
| `Lon` | `double` | Required | - |
| `Id` | `int` | Required | - |
| `DaysOfWeek` | `string` | Optional | - |
| `PreconditionTime` | `int?` | Optional | - |
| `OneTime` | `bool?` | Optional | - |
| `Enabled` | `bool` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "lat": 87.82,
  "lon": 176.92,
  "id": 62,
  "days_of_week": "days_of_week8",
  "precondition_time": 70,
  "one_time": false,
  "enabled": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

