
# Calendar History Response

*This model accepts additional fields of type object.*

## Structure

`CalendarHistoryResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Response` | [`ResponseCalendarHistoryResponse`](../../doc/models/response-calendar-history-response.md) | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "response": {
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
    "total_events": 236,
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

