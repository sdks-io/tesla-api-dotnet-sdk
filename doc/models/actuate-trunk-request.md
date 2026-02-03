
# Actuate Trunk Request

*This model accepts additional fields of type object.*

## Structure

`ActuateTrunkRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `WhichTrunk` | [`WhichTrunk`](../../doc/models/which-trunk.md) | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "which_trunk": "front",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

