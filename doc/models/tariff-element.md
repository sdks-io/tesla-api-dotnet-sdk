
# Tariff Element

*This model accepts additional fields of type object.*

## Structure

`TariffElement`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `PriceComponents` | [`List<PriceComponent>`](../../doc/models/price-component.md) | Optional | - |
| `Restrictions` | `object` | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "price_components": [
    {
      "type": "type2",
      "price": 107.9,
      "step_size": 154.12,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "type": "type2",
      "price": 107.9,
      "step_size": 154.12,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "restrictions": {
    "key0": {
      "key1": "val1",
      "key2": "val2"
    },
    "key1": {
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

