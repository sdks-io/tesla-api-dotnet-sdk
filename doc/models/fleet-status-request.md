
# Fleet Status Request

*This model accepts additional fields of type object.*

## Structure

`FleetStatusRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Vins` | `List<string>` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "vins": [
    "vins6"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

