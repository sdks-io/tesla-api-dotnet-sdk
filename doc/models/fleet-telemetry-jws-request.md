
# Fleet Telemetry Jws Request

*This model accepts additional fields of type object.*

## Structure

`FleetTelemetryJwsRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Token` | `string` | Optional | - |
| `Vins` | `List<string>` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "token": "token8",
  "vins": [
    "vins0",
    "vins9",
    "vins8"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

