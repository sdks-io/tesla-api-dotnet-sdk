# User

User account and settings endpoints

```csharp
UserController userController = client.UserController;
```

## Class Name

`UserController`

## Methods

* [Get Custom Feature Flags for a User](../../doc/controllers/user.md#get-custom-feature-flags-for-a-user)
* [Get Summary of a User S Account](../../doc/controllers/user.md#get-summary-of-a-user-s-account)
* [Get Active Orders for a User](../../doc/controllers/user.md#get-active-orders-for-a-user)
* [Get User S Region and Fleet-Api Base URL](../../doc/controllers/user.md#get-user-s-region-and-fleet-api-base-url)


# Get Custom Feature Flags for a User

```csharp
GetCustomFeatureFlagsForAUserAsync()
```

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.BackupResponse](../../doc/models/backup-response.md).

## Example Usage

```csharp
try
{
    ApiResponse<BackupResponse> result = await userController.GetCustomFeatureFlagsForAUserAsync();
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get Summary of a User S Account

```csharp
GetSummaryOfAUserSAccountAsync()
```

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.MeResponse](../../doc/models/me-response.md).

## Example Usage

```csharp
try
{
    ApiResponse<MeResponse> result = await userController.GetSummaryOfAUserSAccountAsync();
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get Active Orders for a User

```csharp
GetActiveOrdersForAUserAsync()
```

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.OrdersResponse](../../doc/models/orders-response.md).

## Example Usage

```csharp
try
{
    ApiResponse<OrdersResponse> result = await userController.GetActiveOrdersForAUserAsync();
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```


# Get User S Region and Fleet-Api Base URL

```csharp
GetUserSRegionAndFleetApiBaseUrlAsync()
```

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `Data` property of this instance returns the response data which is of type [Models.RegionResponse](../../doc/models/region-response.md).

## Example Usage

```csharp
try
{
    ApiResponse<RegionResponse> result = await userController.GetUserSRegionAndFleetApiBaseUrlAsync();
}
catch (ApiException e)
{
    // TODO: Handle exception here
    Console.WriteLine(e.Message);
}
```

