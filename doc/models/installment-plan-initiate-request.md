
# Installment Plan Initiate Request

## Structure

`InstallmentPlanInitiateRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `AutoCapture` | `Boolean` | Optional | - | Boolean getAutoCapture() | setAutoCapture(Boolean autoCapture) |
| `Attempt3dSecure` | `Boolean` | Optional | - | Boolean getAttempt3dSecure() | setAttempt3dSecure(Boolean attempt3dSecure) |
| `Shopper` | [`ShopperData`](../../doc/models/shopper-data.md) | Optional | - | ShopperData getShopper() | setShopper(ShopperData shopper) |
| `PlanData` | [`PlanDataModel`](../../doc/models/plan-data-model.md) | Optional | - | PlanDataModel getPlanData() | setPlanData(PlanDataModel planData) |
| `BillingAddress` | [`AddressDataModel`](../../doc/models/address-data-model.md) | Optional | - | AddressDataModel getBillingAddress() | setBillingAddress(AddressDataModel billingAddress) |
| `RedirectUrls` | [`InitiateRedirectionEndpointsModel`](../../doc/models/initiate-redirection-endpoints-model.md) | Optional | - | InitiateRedirectionEndpointsModel getRedirectUrls() | setRedirectUrls(InitiateRedirectionEndpointsModel redirectUrls) |
| `UxSettings` | [`UxSettingsModel`](../../doc/models/ux-settings-model.md) | Optional | - | UxSettingsModel getUxSettings() | setUxSettings(UxSettingsModel uxSettings) |
| `EventsEndpoints` | [`EventsEndpointsModel`](../../doc/models/events-endpoints-model.md) | Optional | - | EventsEndpointsModel getEventsEndpoints() | setEventsEndpoints(EventsEndpointsModel eventsEndpoints) |
| `ProcessingData` | [`ProcessingData`](../../doc/models/processing-data.md) | Optional | - | ProcessingData getProcessingData() | setProcessingData(ProcessingData processingData) |

## Example (as JSON)

```json
{
  "AutoCapture": false,
  "Attempt3dSecure": false,
  "Shopper": null,
  "PlanData": null,
  "BillingAddress": null
}
```

