
# Location 1

*This model accepts additional fields of type object.*

## Structure

`Location1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Lat` | `double?` | Optional | - |
| `MLong` | `double?` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "lat": 224.48,
  "long": 54.54,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

