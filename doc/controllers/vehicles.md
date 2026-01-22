# Vehicles

```csharp
VehiclesController vehiclesController = client.VehiclesController;
```

## Class Name

`VehiclesController`

## Methods

* [List Vehicles](../../doc/controllers/vehicles.md#list-vehicles)
* [Get Vehicle](../../doc/controllers/vehicles.md#get-vehicle)
* [Mobile Enabled](../../doc/controllers/vehicles.md#mobile-enabled)
* [Nearby Charging Sites](../../doc/controllers/vehicles.md#nearby-charging-sites)
* [Vehicle Live Data](../../doc/controllers/vehicles.md#vehicle-live-data)
* [Wake up Vehicle](../../doc/controllers/vehicles.md#wake-up-vehicle)
* [Vehicle Specs](../../doc/controllers/vehicles.md#vehicle-specs)
* [Vehicle Options](../../doc/controllers/vehicles.md#vehicle-options)
* [Warranty Details](../../doc/controllers/vehicles.md#warranty-details)
* [Get Allowed Drivers for a Vehicle](../../doc/controllers/vehicles.md#get-allowed-drivers-for-a-vehicle)
* [Remove Driver Access From a Vehicle](../../doc/controllers/vehicles.md#remove-driver-access-from-a-vehicle)
* [Get Eligible Vehicle Subscriptions](../../doc/controllers/vehicles.md#get-eligible-vehicle-subscriptions)
* [Get Eligible Vehicle Upgrades](../../doc/controllers/vehicles.md#get-eligible-vehicle-upgrades)
* [Set Enterprise Payer Roles](../../doc/controllers/vehicles.md#set-enterprise-payer-roles)
* [Get Enterprise Roles for a Vehicle](../../doc/controllers/vehicles.md#get-enterprise-roles-for-a-vehicle)
* [Get Fleet Status for Vehicles](../../doc/controllers/vehicles.md#get-fleet-status-for-vehicles)
* [Create or Update Fleet Telemetry Configuration](../../doc/controllers/vehicles.md#create-or-update-fleet-telemetry-configuration)
* [Get Fleet Telemetry Configuration](../../doc/controllers/vehicles.md#get-fleet-telemetry-configuration)
* [Delete Fleet Telemetry Configuration](../../doc/controllers/vehicles.md#delete-fleet-telemetry-configuration)
* [Configure Fleet Telemetry Using Signed JWS Token](../../doc/controllers/vehicles.md#configure-fleet-telemetry-using-signed-jws-token)
* [Get Fleet Telemetry Errors for a Vehicle](../../doc/controllers/vehicles.md#get-fleet-telemetry-errors-for-a-vehicle)


# List Vehicles

```csharp
ListVehiclesAsync()
```

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.Api1VehiclesResponse](../../doc/models/api-1-vehicles-response.md).

## Example Usage

```csharp
try
{
    ApiResponse<Api1VehiclesResponse> result = await vehiclesController.ListVehiclesAsync();
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get Vehicle

```csharp
GetVehicleAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.Api1VehiclesResponseGetVehicle](../../doc/models/api-1-vehicles-response-get-vehicle.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<Api1VehiclesResponseGetVehicle> result = await vehiclesController.GetVehicleAsync(vehicleTag);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Mobile Enabled

```csharp
MobileEnabledAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.Api1VehiclesMobileEnabledResponse](../../doc/models/api-1-vehicles-mobile-enabled-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<Api1VehiclesMobileEnabledResponse> result = await vehiclesController.MobileEnabledAsync(vehicleTag);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Nearby Charging Sites

```csharp
NearbyChargingSitesAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.Api1VehiclesNearbyChargingSitesResponse](../../doc/models/api-1-vehicles-nearby-charging-sites-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<Api1VehiclesNearbyChargingSitesResponse> result = await vehiclesController.NearbyChargingSitesAsync(vehicleTag);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Vehicle Live Data

```csharp
VehicleLiveDataAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.SiteInfoResponse](../../doc/models/site-info-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<SiteInfoResponse> result = await vehiclesController.VehicleLiveDataAsync(vehicleTag);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Wake up Vehicle

```csharp
WakeUpVehicleAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.Api1VehiclesWakeUpResponse](../../doc/models/api-1-vehicles-wake-up-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<Api1VehiclesWakeUpResponse> result = await vehiclesController.WakeUpVehicleAsync(vehicleTag);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Vehicle Specs

```csharp
VehicleSpecsAsync(
    string vin)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Template, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.SiteInfoResponse](../../doc/models/site-info-response.md).

## Example Usage

```csharp
string vin = "vin6";
try
{
    ApiResponse<SiteInfoResponse> result = await vehiclesController.VehicleSpecsAsync(vin);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Vehicle Options

```csharp
VehicleOptionsAsync(
    string vin)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Query, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.Api1DxVehiclesOptionsResponse](../../doc/models/api-1-dx-vehicles-options-response.md).

## Example Usage

```csharp
string vin = "vin6";
try
{
    ApiResponse<Api1DxVehiclesOptionsResponse> result = await vehiclesController.VehicleOptionsAsync(vin);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Warranty Details

```csharp
WarrantyDetailsAsync()
```

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.Api1DxWarrantyDetailsResponse](../../doc/models/api-1-dx-warranty-details-response.md).

## Example Usage

```csharp
try
{
    ApiResponse<Api1DxWarrantyDetailsResponse> result = await vehiclesController.WarrantyDetailsAsync();
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get Allowed Drivers for a Vehicle

```csharp
GetAllowedDriversForAVehicleAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.DriversResponse](../../doc/models/drivers-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<DriversResponse> result = await vehiclesController.GetAllowedDriversForAVehicleAsync(vehicleTag);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Remove Driver Access From a Vehicle

```csharp
RemoveDriverAccessFromAVehicleAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.SimpleOkResponse](../../doc/models/simple-ok-response.md).

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<SimpleOkResponse> result = await vehiclesController.RemoveDriverAccessFromAVehicleAsync(vehicleTag);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get Eligible Vehicle Subscriptions

```csharp
GetEligibleVehicleSubscriptionsAsync(
    string vin)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Query, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.SiteInfoResponse](../../doc/models/site-info-response.md).

## Example Usage

```csharp
string vin = "vin6";
try
{
    ApiResponse<SiteInfoResponse> result = await vehiclesController.GetEligibleVehicleSubscriptionsAsync(vin);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get Eligible Vehicle Upgrades

```csharp
GetEligibleVehicleUpgradesAsync(
    string vin)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Query, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.SiteInfoResponse](../../doc/models/site-info-response.md).

## Example Usage

```csharp
string vin = "vin6";
try
{
    ApiResponse<SiteInfoResponse> result = await vehiclesController.GetEligibleVehicleUpgradesAsync(vin);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Set Enterprise Payer Roles

```csharp
SetEnterprisePayerRolesAsync(
    string vin,
    Models.EnterprisePayerRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Template, Required | - |
| `body` | [`EnterprisePayerRequest`](../../doc/models/enterprise-payer-request.md) | Body, Required | - |

## Response Type

`Task`

## Example Usage

```csharp
string vin = "vin6";
EnterprisePayerRequest body = new EnterprisePayerRequest
{
    Role = "role0",
};

try
{
    await vehiclesController.SetEnterprisePayerRolesAsync(
        vin,
        body
    );
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get Enterprise Roles for a Vehicle

```csharp
GetEnterpriseRolesForAVehicleAsync(
    string vin)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Template, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type object.

## Example Usage

```csharp
string vin = "vin6";
try
{
    ApiResponse<object> result = await vehiclesController.GetEnterpriseRolesForAVehicleAsync(vin);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get Fleet Status for Vehicles

```csharp
GetFleetStatusForVehiclesAsync(
    Models.FleetStatusRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`FleetStatusRequest`](../../doc/models/fleet-status-request.md) | Body, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type object.

## Example Usage

```csharp
FleetStatusRequest body = new FleetStatusRequest
{
};

try
{
    ApiResponse<object> result = await vehiclesController.GetFleetStatusForVehiclesAsync(body);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Create or Update Fleet Telemetry Configuration

```csharp
CreateOrUpdateFleetTelemetryConfigurationAsync(
    object body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | `object` | Body, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type object.

## Example Usage

```csharp
object body = ApiHelper.JsonDeserialize<object>("{\"key1\":\"val1\",\"key2\":\"val2\"}");
try
{
    ApiResponse<object> result = await vehiclesController.CreateOrUpdateFleetTelemetryConfigurationAsync(body);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get Fleet Telemetry Configuration

```csharp
GetFleetTelemetryConfigurationAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type object.

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<object> result = await vehiclesController.GetFleetTelemetryConfigurationAsync(vehicleTag);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Delete Fleet Telemetry Configuration

```csharp
DeleteFleetTelemetryConfigurationAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type object.

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<object> result = await vehiclesController.DeleteFleetTelemetryConfigurationAsync(vehicleTag);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Configure Fleet Telemetry Using Signed JWS Token

```csharp
ConfigureFleetTelemetryUsingSignedJwsTokenAsync(
    Models.FleetTelemetryJwsRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`FleetTelemetryJwsRequest`](../../doc/models/fleet-telemetry-jws-request.md) | Body, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type object.

## Example Usage

```csharp
FleetTelemetryJwsRequest body = new FleetTelemetryJwsRequest
{
};

try
{
    ApiResponse<object> result = await vehiclesController.ConfigureFleetTelemetryUsingSignedJwsTokenAsync(body);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get Fleet Telemetry Errors for a Vehicle

```csharp
GetFleetTelemetryErrorsForAVehicleAsync(
    string vehicleTag)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type object.

## Example Usage

```csharp
string vehicleTag = "vehicle_tag6";
try
{
    ApiResponse<object> result = await vehiclesController.GetFleetTelemetryErrorsForAVehicleAsync(vehicleTag);
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```

