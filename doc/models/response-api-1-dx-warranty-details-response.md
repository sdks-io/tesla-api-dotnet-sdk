
# Response Api 1 Dx Warranty Details Response

*This model accepts additional fields of type object.*

## Structure

`ResponseApi1DxWarrantyDetailsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `ActiveWarranty` | [`List<WarrantyItem>`](../../doc/models/warranty-item.md) | Optional | - |
| `UpcomingWarranty` | [`List<WarrantyItem>`](../../doc/models/warranty-item.md) | Optional | - |
| `ExpiredWarranty` | [`List<WarrantyItem>`](../../doc/models/warranty-item.md) | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "activeWarranty": [
    {
      "warrantyType": "warrantyType4",
      "warrantyDisplayName": "warrantyDisplayName6",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 200,
      "odometerUnit": "odometerUnit0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "warrantyType": "warrantyType4",
      "warrantyDisplayName": "warrantyDisplayName6",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 200,
      "odometerUnit": "odometerUnit0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "warrantyType": "warrantyType4",
      "warrantyDisplayName": "warrantyDisplayName6",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 200,
      "odometerUnit": "odometerUnit0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "upcomingWarranty": [
    {
      "warrantyType": "warrantyType6",
      "warrantyDisplayName": "warrantyDisplayName8",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 236,
      "odometerUnit": "odometerUnit8",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "warrantyType": "warrantyType6",
      "warrantyDisplayName": "warrantyDisplayName8",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 236,
      "odometerUnit": "odometerUnit8",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "expiredWarranty": [
    {
      "warrantyType": "warrantyType0",
      "warrantyDisplayName": "warrantyDisplayName2",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 38,
      "odometerUnit": "odometerUnit6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "warrantyType": "warrantyType0",
      "warrantyDisplayName": "warrantyDisplayName2",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 38,
      "odometerUnit": "odometerUnit6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "warrantyType": "warrantyType0",
      "warrantyDisplayName": "warrantyDisplayName2",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 38,
      "odometerUnit": "odometerUnit6",
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

