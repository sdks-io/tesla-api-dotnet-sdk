
# Api 1 Dx Vehicles Options Response

*This model accepts additional fields of type object.*

## Structure

`Api1DxVehiclesOptionsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Response` | [`ResponseApi1DxVehiclesOptionsResponse`](../../doc/models/response-api-1-dx-vehicles-options-response.md) | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "response": {
    "codes": [
      {
        "code": "code0",
        "displayName": "displayName0",
        "colorCode": "colorCode2",
        "isActive": false,
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

