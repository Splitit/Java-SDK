
# Getting Started with splitit-web-api-v3

## Install the Package

Install the SDK by adding the following dependency in your project's pom.xml file:

```xml
<dependency>
  <groupId>io.github.splitit</groupId>
  <artifactId>splitit-java-sdk</artifactId>
  <version>4.0.6</version>
</dependency>
```

You can also view the package at:
https://central.sonatype.com/artifact/io.github.splitit/splitit-java-sdk/4.0.6

## Test the SDK

The generated code and the server can be tested using automatically generated test cases.
JUnit is used as the testing framework and test runner.

In Eclipse, for running the tests do the following:

1. Select the project SplititWebApiV3Lib from the package explorer.
2. Select `Run -> Run as -> JUnit Test` or use `Alt + Shift + X` followed by `T` to run the Tests.

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| environment | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| httpClientConfig | [`Consumer<HttpClientConfiguration.Builder>`](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/http-client-configuration-builder.md) | Set up Http Client Configuration instance. |
| oAuth2SandboxCredentials | [`OAuth2SandboxCredentials`](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/auth/oauth-2-client-credentials-grant.md) | The Credentials Setter for OAuth 2 Client Credentials Grant |
| oAuth2ProductionCredentials | [`OAuth2ProductionCredentials`](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/auth/oauth-2-client-credentials-grant-1.md) | The Credentials Setter for OAuth 2 Client Credentials Grant |

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

## Environments

The SDK can be configured to use a different environment for making API calls. Available environments are:

### Fields

| Name | Description |
|  --- | --- |
| production | **Default** Sandbox |
| environment2 | Production |

## Authorization

This API uses the following authentication schemes.

* [`OAuth2-sandbox (OAuth 2 Client Credentials Grant)`](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/auth/oauth-2-client-credentials-grant.md)
* [`OAuth2-production (OAuth 2 Client Credentials Grant)`](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/auth/oauth-2-client-credentials-grant-1.md)

## List of APIs

* [Installment Plan](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/controllers/installment-plan.md)

## SDK Infrastructure

### Configuration

* [Configuration Interface](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/configuration-interface.md)
* [HttpClientConfiguration](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/http-client-configuration.md)
* [HttpClientConfiguration.Builder](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/http-client-configuration-builder.md)
* [HttpProxyConfiguration](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/http-proxy-configuration.md)
* [HttpProxyConfiguration.Builder](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/http-proxy-configuration-builder.md)

### HTTP

* [Headers](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/headers.md)
* [HttpCallback Interface](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/http-callback-interface.md)
* [HttpContext](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/http-context.md)
* [HttpBodyRequest](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/http-body-request.md)
* [HttpRequest](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/http-request.md)
* [HttpResponse](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/http-response.md)
* [HttpStringResponse](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/http-string-response.md)

### Utilities

* [ApiException](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/api-exception.md)
* [ApiHelper](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/api-helper.md)
* [FileWrapper](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/file-wrapper.md)
* [DateTimeHelper](https://www.github.com/Splitit/Java-SDK/tree/4.0.6/doc/date-time-helper.md)

