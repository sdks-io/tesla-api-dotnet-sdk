
# Response Calendar History Response

*This model accepts additional fields of type object.*

## Structure

`ResponseCalendarHistoryResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Events` | [`List<Event>`](../../doc/models/event.md) | Required | - |
| `TotalEvents` | `int` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "events": [
    {
      "timestamp": "2016-03-13T12:52:32.123Z",
      "duration": 68,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "total_events": 12,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

