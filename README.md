
# Getting Started with Tesla Fleet Management API

## Introduction

Unofficial OpenAPI specification for Tesla Fleet Management Charging endpoints.

## Install the Package

If you are building with .NET CLI tools then you can also use the following command:

```bash
dotnet add package TeslaApiSDK --version 1.0.0
```

You can also view the package at:
https://www.nuget.org/packages/TeslaApiSDK/1.0.0

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| Environment | `Environment` | The API environment. <br> **Default: `Environment.Production`** |
| Timeout | `TimeSpan` | Http client timeout.<br>*Default*: `TimeSpan.FromSeconds(100)` |
| HttpClientConfiguration | [`Action<HttpClientConfiguration.Builder>`](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/http-client-configuration-builder.md) | Action delegate that configures the HTTP client by using the HttpClientConfiguration.Builder for customizing API call settings.<br>*Default*: `new HttpClient()` |
| LogBuilder | [`LogBuilder`](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/log-builder.md) | Represents the logging configuration builder for API calls |
| BearerAuthCredentials | [`BearerAuthCredentials`](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/auth/oauth-2-bearer-token.md) | The Credentials Setter for OAuth 2 Bearer token |
| Oauth2Credentials | [`Oauth2Credentials`](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/auth/oauth-2-authorization-code-grant.md) | The Credentials Setter for OAuth 2 Authorization Code Grant |

The API client can be initialized as follows:

### Code-Based Initialization

```csharp
using Microsoft.Extensions.Logging;
using TeslaFleetManagementApi.Standard;
using TeslaFleetManagementApi.Standard.Authentication;

namespace ConsoleApp;

TeslaFleetManagementApiClient client = new TeslaFleetManagementApiClient.Builder()
    .BearerAuthCredentials(
        new BearerAuthModel.Builder(
            "AccessToken"
        )
        .Build())
    .Oauth2Credentials(
        new Oauth2Model.Builder(
            "OAuthClientId",
            "OAuthClientSecret",
            "OAuthRedirectUri"
        )
        .Build())
    .Environment(TeslaFleetManagementApi.Standard.Environment.Production)
    .LoggingConfig(config => config
        .LogLevel(LogLevel.Information)
        .RequestConfig(reqConfig => reqConfig.Body(true))
        .ResponseConfig(respConfig => respConfig.Headers(true))
    )
    .Build();
```

### Configuration-Based Initialization

```csharp
using TeslaFleetManagementApi.Standard;
using Microsoft.Extensions.Configuration;

namespace ConsoleApp;

// Build the IConfiguration using .NET conventions (JSON, environment, etc.)
var configuration = new ConfigurationBuilder()
    .AddJsonFile("config.json")
    .AddEnvironmentVariables() // [optional] read environment variables
    .Build();

// Instantiate your SDK and configure it from IConfiguration
var client = TeslaFleetManagementApiClient
    .FromConfiguration(configuration.GetSection("TeslaFleetManagementApi"));
```

See the [Configuration-Based Initialization](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/configuration-based-initialization.md) section for details.

## Authorization

This API uses the following authentication schemes.

* [`bearerAuth (OAuth 2 Bearer token)`](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/auth/oauth-2-bearer-token.md)
* [`oauth2 (OAuth 2 Authorization Code Grant)`](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/auth/oauth-2-authorization-code-grant.md)

## List of APIs

* [Charging](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/controllers/charging.md)
* [Energy](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/controllers/energy.md)
* [Partner](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/controllers/partner.md)
* [User](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/controllers/user.md)
* [Vehicles](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/controllers/vehicles.md)

## SDK Infrastructure

### Configuration

* [Configuration-Based Initialization](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/configuration-based-initialization.md)
* [HttpClientConfiguration](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/http-client-configuration.md)
* [HttpClientConfigurationBuilder](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/http-client-configuration-builder.md)
* [LogBuilder](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/log-builder.md)
* [LogRequestBuilder](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/log-request-builder.md)
* [LogResponseBuilder](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/log-response-builder.md)
* [ProxyConfigurationBuilder](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/proxy-configuration-builder.md)

### HTTP

* [HttpCallback](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/http-callback.md)
* [HttpContext](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/http-context.md)
* [HttpRequest](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/http-request.md)
* [HttpResponse](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/http-response.md)
* [HttpStringResponse](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/http-string-response.md)

### Utilities

* [ApiException](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/api-exception.md)
* [ApiResponse](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/api-response.md)
* [ApiHelper](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/api-helper.md)
* [CustomDateTimeConverter](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/custom-date-time-converter.md)
* [UnixDateTimeConverter](https://www.github.com/sdks-io/tesla-api-dotnet-sdk/tree/1.0.0/doc/unix-date-time-converter.md)

