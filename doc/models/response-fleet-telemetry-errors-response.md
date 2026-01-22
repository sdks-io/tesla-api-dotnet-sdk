
# Response Fleet Telemetry Errors Response

*This model accepts additional fields of type object.*

## Structure

`ResponseFleetTelemetryErrorsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `FleetTelemetryErrors` | [`List<FleetTelemetryError>`](../../doc/models/fleet-telemetry-error.md) | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "fleet_telemetry_errors": [
    {
      "name": "name8",
      "error": "error2",
      "vin": "vin8",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

