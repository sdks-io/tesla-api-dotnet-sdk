# Partner

Partner account and telemetry endpoints

```csharp
PartnerController partnerController = client.PartnerController;
```

## Class Name

`PartnerController`

## Methods

* [Get Vins With Fleet Telemetry Errors](../../doc/controllers/partner.md#get-vins-with-fleet-telemetry-errors)
* [Get Recent Fleet Telemetry Errors](../../doc/controllers/partner.md#get-recent-fleet-telemetry-errors)
* [Get Public Key for a Domain](../../doc/controllers/partner.md#get-public-key-for-a-domain)
* [Register a Partner Account](../../doc/controllers/partner.md#register-a-partner-account)


# Get Vins With Fleet Telemetry Errors

```csharp
GetVinsWithFleetTelemetryErrorsAsync()
```

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.BackupResponse](../../doc/models/backup-response.md).

## Example Usage

```csharp
try
{
    ApiResponse<BackupResponse> result = await partnerController.GetVinsWithFleetTelemetryErrorsAsync();
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Get Recent Fleet Telemetry Errors

```csharp
GetRecentFleetTelemetryErrorsAsync()
```

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.FleetTelemetryErrorsResponse](../../doc/models/fleet-telemetry-errors-response.md).

## Example Usage

```csharp
try
{
    ApiResponse<FleetTelemetryErrorsResponse> result = await partnerController.GetRecentFleetTelemetryErrorsAsync();
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Get Public Key for a Domain

```csharp
GetPublicKeyForADomainAsync(
    string domain)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `domain` | `string` | Query, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.PublicKeyResponse](../../doc/models/public-key-response.md).

## Example Usage

```csharp
string domain = "domain6";
try
{
    ApiResponse<PublicKeyResponse> result = await partnerController.GetPublicKeyForADomainAsync(domain);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```


# Register a Partner Account

```csharp
RegisterAPartnerAccountAsync(
    Models.RegisterPartnerRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`RegisterPartnerRequest`](../../doc/models/register-partner-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.RegisterPartnerResponse](../../doc/models/register-partner-response.md).

## Example Usage

```csharp
RegisterPartnerRequest body = new RegisterPartnerRequest
{
    Domain = "domain.com",
};

try
{
    ApiResponse<RegisterPartnerResponse> result = await partnerController.RegisterAPartnerAccountAsync(body);
}
catch (ApiException e)
{
    Console.WriteLine(e.Message);
}
```

