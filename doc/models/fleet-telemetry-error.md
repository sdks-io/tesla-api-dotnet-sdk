
# Fleet Telemetry Error

*This model accepts additional fields of type object.*

## Structure

`FleetTelemetryError`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Name` | `string` | Required | - |
| `Error` | `string` | Required | - |
| `Vin` | `string` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "name": "name2",
  "error": "error6",
  "vin": "vin6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

