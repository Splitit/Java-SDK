
# Client Class Documentation

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| environment | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| httpClientConfig | [`Consumer<HttpClientConfiguration.Builder>`](../doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |
| oAuth2SandboxCredentials | [`OAuth2SandboxCredentials`](auth/oauth-2-client-credentials-grant.md) | The Credentials Setter for OAuth 2 Client Credentials Grant |
| oAuth2ProductionCredentials | [`OAuth2ProductionCredentials`](auth/oauth-2-client-credentials-grant-1.md) | The Credentials Setter for OAuth 2 Client Credentials Grant |

The API client can be initialized as follows:

```java
import com.splitit.sandbox.webapiv3.Environment;
import com.splitit.sandbox.webapiv3.SplititWebApiV3Client;
import com.splitit.sandbox.webapiv3.authentication.OAuth2ProductionModel;
import com.splitit.sandbox.webapiv3.authentication.OAuth2SandboxModel;
import com.splitit.sandbox.webapiv3.exceptions.ApiException;
import com.splitit.sandbox.webapiv3.models.OAuthScopeOAuth2ProductionEnum;
import com.splitit.sandbox.webapiv3.models.OAuthScopeOAuth2SandboxEnum;
import com.splitit.sandbox.webapiv3.models.OAuthToken;
import java.io.IOException;
import java.util.Arrays;

public class Program {
    public static void main(String[] args) {
        SplititWebApiV3Client client = new SplititWebApiV3Client.Builder()
            .httpClientConfig(configBuilder -> configBuilder
                    .timeout(0))
            .oAuth2SandboxCredentials(new OAuth2SandboxModel.Builder(
                    "OAuthClientId",
                    "OAuthClientSecret"
                )
                .oAuthScopes(Arrays.asList(
                        OAuthScopeOAuth2SandboxEnum.API_V3
                    ))
                .build())
            .oAuth2ProductionCredentials(new OAuth2ProductionModel.Builder(
                    "OAuthClientId",
                    "OAuthClientSecret"
                )
                .oAuthScopes(Arrays.asList(
                        OAuthScopeOAuth2ProductionEnum.API_V3
                    ))
                .build())
            .environment(Environment.PRODUCTION)
            .build();

    }
}
```

## splitit-web-api-v3Client Class

The gateway for the SDK. This class acts as a factory for the Controllers and also holds the configuration of the SDK.

### Controllers

| Name | Description | Return Type |
|  --- | --- | --- |
| `getInstallmentPlanController()` | Provides access to InstallmentPlan controller. | `InstallmentPlanController` |
| `getOAuthAuthorizationController()` | Provides access to OAuthAuthorization controller. | `OAuthAuthorizationController` |

### Methods

| Name | Description | Return Type |
|  --- | --- | --- |
| `shutdown()` | Shutdown the underlying HttpClient instance. | `void` |
| `getEnvironment()` | Current API environment. | `Environment` |
| `getHttpClient()` | The HTTP Client instance to use for making HTTP requests. | `HttpClient` |
| `getHttpClientConfig()` | Http Client Configuration instance. | [`ReadonlyHttpClientConfiguration`](../doc/http-client-configuration.md) |
| `getOAuth2SandboxCredentials()` | The credentials to use with OAuth2Sandbox. | [`OAuth2SandboxCredentials`](auth/oauth-2-client-credentials-grant.md) |
| `getOAuth2ProductionCredentials()` | The credentials to use with OAuth2Production. | [`OAuth2ProductionCredentials`](auth/oauth-2-client-credentials-grant-1.md) |
| `getBaseUri(Server server)` | Get base URI by current environment | `String` |
| `getBaseUri()` | Get base URI by current environment | `String` |

