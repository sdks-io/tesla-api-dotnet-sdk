# Charging

Charging history, invoices, and session data

```csharp
ChargingController chargingController = client.ChargingController;
```

## Class Name

`ChargingController`

## Methods

* [Get Charging History](../../doc/controllers/charging.md#get-charging-history)
* [Get Charging Invoice](../../doc/controllers/charging.md#get-charging-invoice)
* [Get Charging Sessions](../../doc/controllers/charging.md#get-charging-sessions)


# Get Charging History

Returns the paginated charging history for the authenticated account.

```csharp
GetChargingHistoryAsync()
```

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.ChargingHistoryResponse](../../doc/models/charging-history-response.md).

## Example Usage

```csharp
try
{
    ApiResponse<ChargingHistoryResponse> result = await chargingController.GetChargingHistoryAsync();
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Get Charging Invoice

Returns a charging invoice PDF for a charging session.

```csharp
GetChargingInvoiceAsync(
    string id)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `string` | Template, Required | Charging session invoice identifier |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type dynamic.

## Example Usage

```csharp
string id = "id0";
try
{
    ApiResponse<dynamic> result = await chargingController.GetChargingInvoiceAsync(id);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Get Charging Sessions

Returns charging session information. Only available for business fleet owners.

```csharp
GetChargingSessionsAsync()
```

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.ChargingSessionsResponse](../../doc/models/charging-sessions-response.md).

## Example Usage

```csharp
try
{
    ApiResponse<ChargingSessionsResponse> result = await chargingController.GetChargingSessionsAsync();
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```

