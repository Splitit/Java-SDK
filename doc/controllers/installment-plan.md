# Installment Plan

```java
InstallmentPlanController installmentPlanController = client.getInstallmentPlanController();
```

## Class Name

`InstallmentPlanController`

## Methods

* [Installment Plan Get](../../doc/controllers/installment-plan.md#installment-plan-get)
* [Installment Plan Search](../../doc/controllers/installment-plan.md#installment-plan-search)
* [Installment Plan Post](../../doc/controllers/installment-plan.md#installment-plan-post)
* [Installment Plan Post 2](../../doc/controllers/installment-plan.md#installment-plan-post-2)
* [Installment Plan Verify Authorization](../../doc/controllers/installment-plan.md#installment-plan-verify-authorization)
* [Installment Plan Update Order](../../doc/controllers/installment-plan.md#installment-plan-update-order)
* [Installment Plan Update Order 2](../../doc/controllers/installment-plan.md#installment-plan-update-order-2)
* [Installment Plan Refund](../../doc/controllers/installment-plan.md#installment-plan-refund)
* [Installment Plan Check Eligibility](../../doc/controllers/installment-plan.md#installment-plan-check-eligibility)
* [Installment Plan Get Eligibility Terms and Condition](../../doc/controllers/installment-plan.md#installment-plan-get-eligibility-terms-and-condition)


# Installment Plan Get

```java
CompletableFuture<InstallmentPlanGetResponse> installmentPlanGetAsync(
    final String installmentPlanNumber,
    final String xSplititTouchPoint)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `installmentPlanNumber` | `String` | Template, Required | - |
| `xSplititTouchPoint` | `String` | Header, Optional | TouchPoint |

## Requires scope

### OAuth2-sandbox

`api.v3`

### OAuth2-production

`api.v3`

## Response Type

[`InstallmentPlanGetResponse`](../../doc/models/installment-plan-get-response.md)

## Example Usage

```java
String installmentPlanNumber = "installmentPlanNumber6";

installmentPlanController.installmentPlanGetAsync(installmentPlanNumber, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 403 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 404 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 500 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |


# Installment Plan Search

```java
CompletableFuture<InstallmentPlanSearchResponse> installmentPlanSearchAsync(
    final String installmentPlanNumber,
    final String refOrderNumber,
    final Object extendedParams,
    final String xSplititTouchPoint)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `installmentPlanNumber` | `String` | Query, Optional | - |
| `refOrderNumber` | `String` | Query, Optional | - |
| `extendedParams` | `Object` | Query, Optional | - |
| `xSplititTouchPoint` | `String` | Header, Optional | TouchPoint |

## Requires scope

### OAuth2-sandbox

`api.v3`

### OAuth2-production

`api.v3`

## Response Type

[`InstallmentPlanSearchResponse`](../../doc/models/installment-plan-search-response.md)

## Example Usage

```java
installmentPlanController.installmentPlanSearchAsync(null, null, null, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 403 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 404 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 500 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |


# Installment Plan Post

```java
CompletableFuture<InitiatePlanResponse> installmentPlanPostAsync(
    final String xSplititIdempotencyKey,
    final InstallmentPlanInitiateRequest body,
    final TestModesEnum xSplititTestMode,
    final String xSplititTouchPoint)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `xSplititIdempotencyKey` | `String` | Header, Required | - |
| `body` | [`InstallmentPlanInitiateRequest`](../../doc/models/installment-plan-initiate-request.md) | Body, Required | - |
| `xSplititTestMode` | [`TestModesEnum`](../../doc/models/test-modes-enum.md) | Header, Optional | - |
| `xSplititTouchPoint` | `String` | Header, Optional | TouchPoint |

## Requires scope

### OAuth2-sandbox

`api.v3`

### OAuth2-production

`api.v3`

## Response Type

[`InitiatePlanResponse`](../../doc/models/initiate-plan-response.md)

## Example Usage

```java
String xSplititIdempotencyKey = "X-Splitit-IdempotencyKey2";
InstallmentPlanInitiateRequest body = new InstallmentPlanInitiateRequest.Builder()
    .build();


installmentPlanController.installmentPlanPostAsync(xSplititIdempotencyKey, body, null, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 400 | - | [`PlanErrorResponseException`](../../doc/models/plan-error-response-exception.md) |
| 401 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 403 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 404 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 500 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |


# Installment Plan Post 2

```java
CompletableFuture<InstallmentPlanCreateResponse> installmentPlanPost2Async(
    final String xSplititIdempotencyKey,
    final InstallmentPlanCreateRequest body,
    final TestModesEnum xSplititTestMode,
    final String xSplititTouchPoint)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `xSplititIdempotencyKey` | `String` | Header, Required | - |
| `body` | [`InstallmentPlanCreateRequest`](../../doc/models/installment-plan-create-request.md) | Body, Required | - |
| `xSplititTestMode` | [`TestModesEnum`](../../doc/models/test-modes-enum.md) | Header, Optional | - |
| `xSplititTouchPoint` | `String` | Header, Optional | TouchPoint |

## Requires scope

### OAuth2-sandbox

`api.v3`

### OAuth2-production

`api.v3`

## Response Type

[`InstallmentPlanCreateResponse`](../../doc/models/installment-plan-create-response.md)

## Example Usage

```java
String xSplititIdempotencyKey = "X-Splitit-IdempotencyKey2";
InstallmentPlanCreateRequest body = new InstallmentPlanCreateRequest.Builder(
    false,
    false
)
.build();


installmentPlanController.installmentPlanPost2Async(xSplititIdempotencyKey, body, null, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 400 | - | [`PlanErrorResponseException`](../../doc/models/plan-error-response-exception.md) |
| 401 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 403 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 404 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 500 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |


# Installment Plan Verify Authorization

```java
CompletableFuture<VerifyAuthorizationResponse> installmentPlanVerifyAuthorizationAsync(
    final String installmentPlanNumber,
    final String xSplititTouchPoint)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `installmentPlanNumber` | `String` | Template, Required | - |
| `xSplititTouchPoint` | `String` | Header, Optional | TouchPoint |

## Requires scope

### OAuth2-sandbox

`api.v3`

### OAuth2-production

`api.v3`

## Response Type

[`VerifyAuthorizationResponse`](../../doc/models/verify-authorization-response.md)

## Example Usage

```java
String installmentPlanNumber = "installmentPlanNumber6";

installmentPlanController.installmentPlanVerifyAuthorizationAsync(installmentPlanNumber, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 403 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 404 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 500 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |


# Installment Plan Update Order

```java
CompletableFuture<InstallmentPlanUpdateResponse> installmentPlanUpdateOrderAsync(
    final String installmentPlanNumber,
    final String xSplititIdempotencyKey,
    final InstallmentPlanUpdateRequest body,
    final String xSplititTouchPoint)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `installmentPlanNumber` | `String` | Template, Required | - |
| `xSplititIdempotencyKey` | `String` | Header, Required | - |
| `body` | [`InstallmentPlanUpdateRequest`](../../doc/models/installment-plan-update-request.md) | Body, Required | - |
| `xSplititTouchPoint` | `String` | Header, Optional | TouchPoint |

## Requires scope

### OAuth2-sandbox

`api.v3`

### OAuth2-production

`api.v3`

## Response Type

[`InstallmentPlanUpdateResponse`](../../doc/models/installment-plan-update-response.md)

## Example Usage

```java
String installmentPlanNumber = "installmentPlanNumber6";
String xSplititIdempotencyKey = "X-Splitit-IdempotencyKey2";
InstallmentPlanUpdateRequest body = new InstallmentPlanUpdateRequest.Builder()
    .build();


installmentPlanController.installmentPlanUpdateOrderAsync(installmentPlanNumber, xSplititIdempotencyKey, body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 403 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 404 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 500 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |


# Installment Plan Update Order 2

```java
CompletableFuture<InstallmentPlanUpdateResponse> installmentPlanUpdateOrder2Async(
    final String xSplititIdempotencyKey,
    final InstallmentPlanUpdateRequestByIdentifier body,
    final String xSplititTouchPoint)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `xSplititIdempotencyKey` | `String` | Header, Required | - |
| `body` | [`InstallmentPlanUpdateRequestByIdentifier`](../../doc/models/installment-plan-update-request-by-identifier.md) | Body, Required | - |
| `xSplititTouchPoint` | `String` | Header, Optional | TouchPoint |

## Requires scope

### OAuth2-sandbox

`api.v3`

### OAuth2-production

`api.v3`

## Response Type

[`InstallmentPlanUpdateResponse`](../../doc/models/installment-plan-update-response.md)

## Example Usage

```java
String xSplititIdempotencyKey = "X-Splitit-IdempotencyKey2";
InstallmentPlanUpdateRequestByIdentifier body = new InstallmentPlanUpdateRequestByIdentifier.Builder()
    .build();


installmentPlanController.installmentPlanUpdateOrder2Async(xSplititIdempotencyKey, body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 403 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 404 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 500 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |


# Installment Plan Refund

```java
CompletableFuture<InstallmentPlanRefundResponse> installmentPlanRefundAsync(
    final String installmentPlanNumber,
    final String xSplititIdempotencyKey,
    final InstallmentPlanRefundRequest body,
    final String xSplititTouchPoint)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `installmentPlanNumber` | `String` | Template, Required | - |
| `xSplititIdempotencyKey` | `String` | Header, Required | - |
| `body` | [`InstallmentPlanRefundRequest`](../../doc/models/installment-plan-refund-request.md) | Body, Required | - |
| `xSplititTouchPoint` | `String` | Header, Optional | TouchPoint |

## Requires scope

### OAuth2-sandbox

`api.v3`

### OAuth2-production

`api.v3`

## Response Type

[`InstallmentPlanRefundResponse`](../../doc/models/installment-plan-refund-response.md)

## Example Usage

```java
String installmentPlanNumber = "installmentPlanNumber6";
String xSplititIdempotencyKey = "X-Splitit-IdempotencyKey2";
InstallmentPlanRefundRequest body = new InstallmentPlanRefundRequest.Builder(
    "Amount8"
)
.build();


installmentPlanController.installmentPlanRefundAsync(installmentPlanNumber, xSplititIdempotencyKey, body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 403 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 404 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 500 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |


# Installment Plan Check Eligibility

```java
CompletableFuture<InstallmentsEligibilityResponse> installmentPlanCheckEligibilityAsync(
    final String xSplititIdempotencyKey,
    final CheckInstallmentsEligibilityRequest body,
    final String xSplititTouchPoint)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `xSplititIdempotencyKey` | `String` | Header, Required | - |
| `body` | [`CheckInstallmentsEligibilityRequest`](../../doc/models/check-installments-eligibility-request.md) | Body, Required | - |
| `xSplititTouchPoint` | `String` | Header, Optional | TouchPoint |

## Requires scope

### OAuth2-sandbox

`api.v3`

### OAuth2-production

`api.v3`

## Response Type

[`InstallmentsEligibilityResponse`](../../doc/models/installments-eligibility-response.md)

## Example Usage

```java
String xSplititIdempotencyKey = "X-Splitit-IdempotencyKey2";
CheckInstallmentsEligibilityRequest body = new CheckInstallmentsEligibilityRequest.Builder()
    .build();


installmentPlanController.installmentPlanCheckEligibilityAsync(xSplititIdempotencyKey, body, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 403 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 404 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 500 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |


# Installment Plan Get Eligibility Terms and Condition

```java
CompletableFuture<EligibilityTermsAndConditionResponse> installmentPlanGetEligibilityTermsAndConditionAsync(
    final String ipn,
    final String xSplititTouchPoint)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `ipn` | `String` | Template, Required | - |
| `xSplititTouchPoint` | `String` | Header, Optional | TouchPoint |

## Requires scope

### OAuth2-sandbox

`api.v3`

### OAuth2-production

`api.v3`

## Response Type

[`EligibilityTermsAndConditionResponse`](../../doc/models/eligibility-terms-and-condition-response.md)

## Example Usage

```java
String ipn = "ipn4";

installmentPlanController.installmentPlanGetEligibilityTermsAndConditionAsync(ipn, null).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 403 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 404 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |
| 500 | - | [`FailedResponseException`](../../doc/models/failed-response-exception.md) |

