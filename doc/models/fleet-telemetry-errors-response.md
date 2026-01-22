
# Fleet Telemetry Errors Response

*This model accepts additional fields of type object.*

## Structure

`FleetTelemetryErrorsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Response` | [`ResponseFleetTelemetryErrorsResponse`](../../doc/models/response-fleet-telemetry-errors-response.md) | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "response": {
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
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

