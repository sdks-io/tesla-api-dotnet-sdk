
# Client Class Documentation

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| Environment | `Environment` | The API environment. <br> **Default: `Environment.Production`** |
| Timeout | `TimeSpan` | Http client timeout.<br>*Default*: `TimeSpan.FromSeconds(100)` |
| HttpClientConfiguration | [`Action<HttpClientConfiguration.Builder>`](../doc/http-client-configuration-builder.md) | Action delegate that configures the HTTP client by using the HttpClientConfiguration.Builder for customizing API call settings.<br>*Default*: `new HttpClient()` |
| LogBuilder | [`LogBuilder`](../doc/log-builder.md) | Represents the logging configuration builder for API calls |
| BearerAuthCredentials | [`BearerAuthCredentials`](auth/oauth-2-bearer-token.md) | The Credentials Setter for OAuth 2 Bearer token |
| Oauth2Credentials | [`Oauth2Credentials`](auth/oauth-2-authorization-code-grant.md) | The Credentials Setter for OAuth 2 Authorization Code Grant |

The API client can be initialized as follows:

## Code-Based Initialization

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

## Configuration-Based Initialization

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

See the [Configuration-Based Initialization](../doc/configuration-based-initialization.md) section for details.

## Tesla Fleet Management APIClient Class

The gateway for the SDK. This class acts as a factory for the Controllers and also holds the configuration of the SDK.

### Controllers

| Name | Description |
|  --- | --- |
| ChargingController | Gets ChargingController controller. |
| EnergyController | Gets EnergyController controller. |
| PartnerController | Gets PartnerController controller. |
| UserController | Gets UserController controller. |
| VehiclesController | Gets VehiclesController controller. |
| OauthAuthorizationController | Gets OauthAuthorizationController controller. |

### Properties

| Name | Description | Type |
|  --- | --- | --- |
| HttpClientConfiguration | Gets the configuration of the Http Client associated with this client. | [`IHttpClientConfiguration`](../doc/http-client-configuration.md) |
| Timeout | Http client timeout. | `TimeSpan` |
| Environment | Current API environment. | `Environment` |
| BearerAuthCredentials | Gets the credentials to use with BearerAuth. | [`IBearerAuthCredentials`](auth/oauth-2-bearer-token.md) |
| Oauth2Credentials | Gets the credentials to use with Oauth2. | [`IOauth2Credentials`](auth/oauth-2-authorization-code-grant.md) |

### Methods

| Name | Description | Return Type |
|  --- | --- | --- |
| `GetBaseUri(Server alias = Server.Default)` | Gets the URL for a particular alias in the current environment and appends it with template parameters. | `string` |
| `ToBuilder()` | Creates an object of the Tesla Fleet Management APIClient using the values provided for the builder. | `Builder` |

## Tesla Fleet Management APIClient Builder Class

Class to build instances of Tesla Fleet Management APIClient.

### Methods

| Name | Description | Return Type |
|  --- | --- | --- |
| `HttpClientConfiguration(Action<`[`HttpClientConfiguration.Builder`](../doc/http-client-configuration-builder.md)`> action)` | Gets the configuration of the Http Client associated with this client. | `Builder` |
| `Timeout(TimeSpan timeout)` | Http client timeout. | `Builder` |
| `Environment(Environment environment)` | Current API environment. | `Builder` |
| `BearerAuthCredentials(Action<BearerAuthModel.Builder> action)` | Sets credentials for BearerAuth. | `Builder` |
| `Oauth2Credentials(Action<Oauth2Model.Builder> action)` | Sets credentials for Oauth2. | `Builder` |

