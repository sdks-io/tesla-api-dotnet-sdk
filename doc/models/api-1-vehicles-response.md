
# Api 1 Vehicles Response

*This model accepts additional fields of type object.*

## Structure

`Api1VehiclesResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Response` | [`List<VehicleBase>`](../../doc/models/vehicle-base.md) | Optional | - |
| `Pagination` | [`Pagination`](../../doc/models/pagination.md) | Optional | - |
| `Count` | `int?` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "response": [
    {
      "id": 206,
      "vehicle_id": 56,
      "vin": "vin6",
      "display_name": "display_name0",
      "access_type": "access_type4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "pagination": {
    "previous": 66,
    "next": 156,
    "current": 130,
    "per_page": 54,
    "count": 192,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "count": 14,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

