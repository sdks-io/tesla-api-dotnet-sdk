# Vehicle Commands

```csharp
VehicleCommandsController vehicleCommandsController = client.VehicleCommandsController;
```

## Class Name

`VehicleCommandsController`

## Methods

* [Actuate Trunk](../../doc/controllers/vehicle-commands.md#actuate-trunk)
* [Add Charge Schedule](../../doc/controllers/vehicle-commands.md#add-charge-schedule)
* [Add Precondition Schedule](../../doc/controllers/vehicle-commands.md#add-precondition-schedule)
* [Adjust Media Volume](../../doc/controllers/vehicle-commands.md#adjust-media-volume)
* [Start Climate Preconditioning](../../doc/controllers/vehicle-commands.md#start-climate-preconditioning)
* [Stop Climate Preconditioning](../../doc/controllers/vehicle-commands.md#stop-climate-preconditioning)
* [Cancel Software Update](../../doc/controllers/vehicle-commands.md#cancel-software-update)
* [Charge Max Range](../../doc/controllers/vehicle-commands.md#charge-max-range)
* [Open Charge Port Door](../../doc/controllers/vehicle-commands.md#open-charge-port-door)
* [Close Charge Port Door](../../doc/controllers/vehicle-commands.md#close-charge-port-door)
* [Charge Standard](../../doc/controllers/vehicle-commands.md#charge-standard)
* [Start Charging](../../doc/controllers/vehicle-commands.md#start-charging)
* [Stop Charging](../../doc/controllers/vehicle-commands.md#stop-charging)
* [Clear PIN to Drive Admin](../../doc/controllers/vehicle-commands.md#clear-pin-to-drive-admin)
* [Lock Doors](../../doc/controllers/vehicle-commands.md#lock-doors)
* [Unlock Doors](../../doc/controllers/vehicle-commands.md#unlock-doors)
* [Erase User Data](../../doc/controllers/vehicle-commands.md#erase-user-data)
* [Flash Lights](../../doc/controllers/vehicle-commands.md#flash-lights)
* [Enable or Disable Guest Mode](../../doc/controllers/vehicle-commands.md#enable-or-disable-guest-mode)
* [Honk Horn](../../doc/controllers/vehicle-commands.md#honk-horn)
* [Next Favorite Media Track](../../doc/controllers/vehicle-commands.md#next-favorite-media-track)


# Actuate Trunk

Controls the front or rear trunk

```csharp
ActuateTrunkAsync(
    string vehicleTag,
    Models.ActuateTrunkRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`ActuateTrunkRequest`](../../doc/models/actuate-trunk-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
ActuateTrunkRequest body = new ActuateTrunkRequest
{
    WhichTrunk = WhichTrunk.Front,
};

try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.ActuateTrunkAsync(
        vehicleTag,
        body
    );
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Add Charge Schedule

```csharp
AddChargeScheduleAsync(
    string vehicleTag,
    Models.AddChargeScheduleRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`AddChargeScheduleRequest`](../../doc/models/add-charge-schedule-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
AddChargeScheduleRequest body = new AddChargeScheduleRequest
{
    Lat = 213.84,
    Lon = 209.06,
    Id = 120,
    Enabled = false,
};

try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.AddChargeScheduleAsync(
        vehicleTag,
        body
    );
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Add Precondition Schedule

```csharp
AddPreconditionScheduleAsync(
    string vehicleTag,
    Models.AddPreconditionScheduleRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`AddPreconditionScheduleRequest`](../../doc/models/add-precondition-schedule-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
AddPreconditionScheduleRequest body = new AddPreconditionScheduleRequest
{
    Lat = 213.84,
    Lon = 209.06,
    Id = 120,
    Enabled = false,
};

try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.AddPreconditionScheduleAsync(
        vehicleTag,
        body
    );
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Adjust Media Volume

```csharp
AdjustMediaVolumeAsync(
    string vehicleTag,
    Models.AdjustVolumeRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`AdjustVolumeRequest`](../../doc/models/adjust-volume-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
AdjustVolumeRequest body = new AdjustVolumeRequest
{
    Volume = 74,
};

try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.AdjustMediaVolumeAsync(
        vehicleTag,
        body
    );
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Start Climate Preconditioning

```csharp
StartClimatePreconditioningAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.StartClimatePreconditioningAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Stop Climate Preconditioning

```csharp
StopClimatePreconditioningAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.StopClimatePreconditioningAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Cancel Software Update

```csharp
CancelSoftwareUpdateAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.CancelSoftwareUpdateAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Charge Max Range

```csharp
ChargeMaxRangeAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.ChargeMaxRangeAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Open Charge Port Door

```csharp
OpenChargePortDoorAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.OpenChargePortDoorAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Close Charge Port Door

```csharp
CloseChargePortDoorAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.CloseChargePortDoorAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Charge Standard

```csharp
ChargeStandardAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.ChargeStandardAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Start Charging

```csharp
StartChargingAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.StartChargingAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Stop Charging

```csharp
StopChargingAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.StopChargingAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Clear PIN to Drive Admin

Deactivates PIN to Drive and resets the associated PIN for supported firmware versions.

```csharp
ClearPinToDriveAdminAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.ClearPinToDriveAdminAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Lock Doors

```csharp
LockDoorsAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.LockDoorsAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Unlock Doors

```csharp
UnlockDoorsAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.UnlockDoorsAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Erase User Data

Erases user data from the vehicle UI. Requires Guest Mode.

```csharp
EraseUserDataAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.EraseUserDataAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Flash Lights

Briefly flashes vehicle headlights.

```csharp
FlashLightsAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.FlashLightsAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Enable or Disable Guest Mode

```csharp
EnableOrDisableGuestModeAsync(
    string vehicleTag,
    Models.GuestModeRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`GuestModeRequest`](../../doc/models/guest-mode-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
GuestModeRequest body = new GuestModeRequest
{
    Enable = false,
};

try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.EnableOrDisableGuestModeAsync(
        vehicleTag,
        body
    );
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Honk Horn

```csharp
HonkHornAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.HonkHornAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Next Favorite Media Track

```csharp
NextFavoriteMediaTrackAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CommandResponse](../../doc/models/command-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<CommandResponse> result = await vehicleCommandsController.NextFavoriteMediaTrackAsync(vehicleTag);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```

