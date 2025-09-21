
# Installment Plan Create Request

## Structure

`InstallmentPlanCreateRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AutoCapture` | `boolean` | Required | - | boolean getAutoCapture() | setAutoCapture(boolean autoCapture) |
| `Attempt3dSecure` | `Boolean` | Optional | - | Boolean getAttempt3dSecure() | setAttempt3dSecure(Boolean attempt3dSecure) |
| `TermsAndConditionsAccepted` | `boolean` | Required | - | boolean getTermsAndConditionsAccepted() | setTermsAndConditionsAccepted(boolean termsAndConditionsAccepted) |
| `Shopper` | [`ShopperData`](../../doc/models/shopper-data.md) | Optional | - | ShopperData getShopper() | setShopper(ShopperData shopper) |
| `PlanData` | [`PlanDataModel`](../../doc/models/plan-data-model.md) | Optional | - | PlanDataModel getPlanData() | setPlanData(PlanDataModel planData) |
| `BillingAddress` | [`AddressDataModel`](../../doc/models/address-data-model.md) | Optional | - | AddressDataModel getBillingAddress() | setBillingAddress(AddressDataModel billingAddress) |
| `PaymentMethod` | [`PaymentMethodModel`](../../doc/models/payment-method-model.md) | Optional | - | PaymentMethodModel getPaymentMethod() | setPaymentMethod(PaymentMethodModel paymentMethod) |
| `RedirectUrls` | [`RedirectionEndpointsModel`](../../doc/models/redirection-endpoints-model.md) | Optional | - | RedirectionEndpointsModel getRedirectUrls() | setRedirectUrls(RedirectionEndpointsModel redirectUrls) |
| `ProcessingData` | [`ProcessingData`](../../doc/models/processing-data.md) | Optional | - | ProcessingData getProcessingData() | setProcessingData(ProcessingData processingData) |
| `EventsEndpoints` | [`EventsEndpointsModel`](../../doc/models/events-endpoints-model.md) | Optional | - | EventsEndpointsModel getEventsEndpoints() | setEventsEndpoints(EventsEndpointsModel eventsEndpoints) |

## Example (as JSON)

```json
{
  "AutoCapture": false,
  "Attempt3dSecure": false,
  "TermsAndConditionsAccepted": false,
  "Shopper": null,
  "PlanData": null,
  "BillingAddress": null,
  "PaymentMethod": null
}
```

