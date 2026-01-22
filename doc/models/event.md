
# Event

*This model accepts additional fields of type object.*

## Structure

`Event`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Timestamp` | `DateTime` | Required | - |
| `Duration` | `int` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "timestamp": "2016-03-13T12:52:32.123Z",
  "duration": 40,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

