
# Tariffs

*This model accepts additional fields of type object.*

## Structure

`Tariffs`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Currency` | `string` | Optional | - |
| `Elements` | [`List<TariffElement>`](../../doc/models/tariff-element.md) | Optional | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "currency": "currency0",
  "elements": [
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
        },
        "key2": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
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
        },
        "key2": {
          "key1": "val1",
          "key2": "val2"
        }
      },
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

