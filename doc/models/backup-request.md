
# Backup Request

*This model accepts additional fields of type object.*

## Structure

`BackupRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `BackupReservePercent` | `int` | Required | - |
| `AdditionalProperties` | `object this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "backup_reserve_percent": 32,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

