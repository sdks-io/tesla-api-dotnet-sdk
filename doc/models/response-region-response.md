
# Response Region Response

*This model accepts additional fields of type object.*

## Structure

`ResponseRegionResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Region` | `string` | Required | - |
| `FleetApiBaseUrl` | `string` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "region": "region0",
  "fleet_api_base_url": "fleet_api_base_url8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

