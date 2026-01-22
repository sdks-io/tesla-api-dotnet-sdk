# Energy

Energy site and Powerwall endpoints

```csharp
EnergyController energyController = client.EnergyController;
```

## Class Name

`EnergyController`

## Methods

* [Adjust Site S Backup Reserve](../../doc/controllers/energy.md#adjust-site-s-backup-reserve)
* [Get Backup or Energy History](../../doc/controllers/energy.md#get-backup-or-energy-history)
* [Get Wall Connector Charging History](../../doc/controllers/energy.md#get-wall-connector-charging-history)
* [Get Live Site Status](../../doc/controllers/energy.md#get-live-site-status)
* [Set Site Mode Autonomous or Self Consumption](../../doc/controllers/energy.md#set-site-mode-autonomous-or-self-consumption)
* [Allow Disallow Charging From the Grid and Exporting Energy to the Grid](../../doc/controllers/energy.md#allow-disallow-charging-from-the-grid-and-exporting-energy-to-the-grid)
* [Adjust Site S Off-Grid Vehicle Charging Reserve](../../doc/controllers/energy.md#adjust-site-s-off-grid-vehicle-charging-reserve)
* [Update Storm Watch Participation](../../doc/controllers/energy.md#update-storm-watch-participation)
* [Update Time-of-Use TOU Settings](../../doc/controllers/energy.md#update-time-of-use-tou-settings)
* [Get User Products Vehicles Energy Sites](../../doc/controllers/energy.md#get-user-products-vehicles-energy-sites)
* [Get Site Information Assets Settings Features](../../doc/controllers/energy.md#get-site-information-assets-settings-features)


# Adjust Site S Backup Reserve

```csharp
AdjustSiteSBackupReserveAsync(
    string energySiteId,
    Models.BackupRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`BackupRequest`](../../doc/models/backup-request.md) | Body, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.BackupResponse](../../doc/models/backup-response.md).

## Example Usage

```csharp
string energySiteId = "energy_site_id2";
BackupRequest body = new BackupRequest
{
    BackupReservePercent = 76,
};

try
{
    ApiResponse<BackupResponse> result = await energyController.AdjustSiteSBackupReserveAsync(
        energySiteId,
        body
    );
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get Backup or Energy History

```csharp
GetBackupOrEnergyHistoryAsync(
    string energySiteId,
    Models.Kind kind,
    DateTime startDate,
    DateTime endDate,
    string period = null,
    string timeZone = null)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `kind` | [`Kind`](../../doc/models/kind.md) | Query, Required | - |
| `startDate` | `DateTime` | Query, Required | - |
| `endDate` | `DateTime` | Query, Required | - |
| `period` | `string` | Query, Optional | - |
| `timeZone` | `string` | Query, Optional | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.CalendarHistoryResponse](../../doc/models/calendar-history-response.md).

## Example Usage

```csharp
string energySiteId = "energy_site_id2";
Kind kind = Kind.Backup;
DateTime startDate = DateTime.ParseExact("2016-03-13T12:52:32.123Z", "yyyy'-'MM'-'dd'T'HH':'mm':'ss.FFFFFFFK",
        provider: CultureInfo.InvariantCulture,
        DateTimeStyles.RoundtripKind);
DateTime endDate = DateTime.ParseExact("2016-03-13T12:52:32.123Z", "yyyy'-'MM'-'dd'T'HH':'mm':'ss.FFFFFFFK",
        provider: CultureInfo.InvariantCulture,
        DateTimeStyles.RoundtripKind);
try
{
    ApiResponse<CalendarHistoryResponse> result = await energyController.GetBackupOrEnergyHistoryAsync(
        energySiteId,
        kind,
        startDate,
        endDate
    );
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get Wall Connector Charging History

```csharp
GetWallConnectorChargingHistoryAsync(
    string energySiteId,
    Models.KindGetWallConnectorChargingHistory kind,
    DateTime startDate,
    DateTime endDate,
    string timeZone = null)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `kind` | [`KindGetWallConnectorChargingHistory`](../../doc/models/kind-get-wall-connector-charging-history.md) | Query, Required | - |
| `startDate` | `DateTime` | Query, Required | - |
| `endDate` | `DateTime` | Query, Required | - |
| `timeZone` | `string` | Query, Optional | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.ChargeHistoryResponse](../../doc/models/charge-history-response.md).

## Example Usage

```csharp
string energySiteId = "energy_site_id2";
KindGetWallConnectorChargingHistory kind = KindGetWallConnectorChargingHistory.Charge;
DateTime startDate = DateTime.ParseExact("2016-03-13T12:52:32.123Z", "yyyy'-'MM'-'dd'T'HH':'mm':'ss.FFFFFFFK",
        provider: CultureInfo.InvariantCulture,
        DateTimeStyles.RoundtripKind);
DateTime endDate = DateTime.ParseExact("2016-03-13T12:52:32.123Z", "yyyy'-'MM'-'dd'T'HH':'mm':'ss.FFFFFFFK",
        provider: CultureInfo.InvariantCulture,
        DateTimeStyles.RoundtripKind);
try
{
    ApiResponse<ChargeHistoryResponse> result = await energyController.GetWallConnectorChargingHistoryAsync(
        energySiteId,
        kind,
        startDate,
        endDate
    );
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get Live Site Status

```csharp
GetLiveSiteStatusAsync(
    string energySiteId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.LiveStatusResponse](../../doc/models/live-status-response.md).

## Example Usage

```csharp
string energySiteId = "energy_site_id2";
try
{
    ApiResponse<LiveStatusResponse> result = await energyController.GetLiveSiteStatusAsync(energySiteId);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Set Site Mode Autonomous or Self Consumption

```csharp
SetSiteModeAutonomousOrSelfConsumptionAsync(
    string energySiteId,
    Models.OperationRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`OperationRequest`](../../doc/models/operation-request.md) | Body, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.GenericUpdateResponse](../../doc/models/generic-update-response.md).

## Example Usage

```csharp
string energySiteId = "energy_site_id2";
OperationRequest body = new OperationRequest
{
    DefaultRealMode = DefaultRealMode.Autonomous,
};

try
{
    ApiResponse<GenericUpdateResponse> result = await energyController.SetSiteModeAutonomousOrSelfConsumptionAsync(
        energySiteId,
        body
    );
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Allow Disallow Charging From the Grid and Exporting Energy to the Grid

```csharp
AllowDisallowChargingFromTheGridAndExportingEnergyToTheGridAsync(
    string energySiteId,
    object body = null)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | `object` | Body, Optional | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.GenericUpdateResponse](../../doc/models/generic-update-response.md).

## Example Usage

```csharp
string energySiteId = "energy_site_id2";
try
{
    ApiResponse<GenericUpdateResponse> result = await energyController.AllowDisallowChargingFromTheGridAndExportingEnergyToTheGridAsync(energySiteId);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Adjust Site S Off-Grid Vehicle Charging Reserve

```csharp
AdjustSiteSOffGridVehicleChargingReserveAsync(
    string energySiteId,
    Models.OffGridVehicleChargingReserveRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`OffGridVehicleChargingReserveRequest`](../../doc/models/off-grid-vehicle-charging-reserve-request.md) | Body, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.GenericUpdateResponse](../../doc/models/generic-update-response.md).

## Example Usage

```csharp
string energySiteId = "energy_site_id2";
OffGridVehicleChargingReserveRequest body = new OffGridVehicleChargingReserveRequest
{
    OffGridVehicleChargingReservePercent = 52,
};

try
{
    ApiResponse<GenericUpdateResponse> result = await energyController.AdjustSiteSOffGridVehicleChargingReserveAsync(
        energySiteId,
        body
    );
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Update Storm Watch Participation

```csharp
UpdateStormWatchParticipationAsync(
    string energySiteId,
    Models.StormModeRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`StormModeRequest`](../../doc/models/storm-mode-request.md) | Body, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.GenericUpdateResponse](../../doc/models/generic-update-response.md).

## Example Usage

```csharp
string energySiteId = "energy_site_id2";
StormModeRequest body = new StormModeRequest
{
    Enabled = false,
};

try
{
    ApiResponse<GenericUpdateResponse> result = await energyController.UpdateStormWatchParticipationAsync(
        energySiteId,
        body
    );
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Update Time-of-Use TOU Settings

```csharp
UpdateTimeOfUseTouSettingsAsync(
    string energySiteId,
    Models.TimeOfUseSettingsRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`TimeOfUseSettingsRequest`](../../doc/models/time-of-use-settings-request.md) | Body, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.GenericUpdateResponse](../../doc/models/generic-update-response.md).

## Example Usage

```csharp
string energySiteId = "energy_site_id2";
TimeOfUseSettingsRequest body = new TimeOfUseSettingsRequest
{
    TouSettings = new TouSettings
    {
    },
};

try
{
    ApiResponse<GenericUpdateResponse> result = await energyController.UpdateTimeOfUseTouSettingsAsync(
        energySiteId,
        body
    );
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get User Products Vehicles Energy Sites

```csharp
GetUserProductsVehiclesEnergySitesAsync()
```

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.ProductsResponse](../../doc/models/products-response.md).

## Example Usage

```csharp
try
{
    ApiResponse<ProductsResponse> result = await energyController.GetUserProductsVehiclesEnergySitesAsync();
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get Site Information Assets Settings Features

```csharp
GetSiteInformationAssetsSettingsFeaturesAsync(
    string energySiteId)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.SiteInfoResponse](../../doc/models/site-info-response.md).

## Example Usage

```csharp
string energySiteId = "energy_site_id2";
try
{
    ApiResponse<SiteInfoResponse> result = await energyController.GetSiteInformationAssetsSettingsFeaturesAsync(energySiteId);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```

