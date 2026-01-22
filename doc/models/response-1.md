
# Response 1

*This model accepts additional fields of type object.*

## Structure

`Response1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `FleetTelemetryErrorVins` | `List<string>` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "fleet_telemetry_error_vins": [
    "fleet_telemetry_error_vins1",
    "fleet_telemetry_error_vins2"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

