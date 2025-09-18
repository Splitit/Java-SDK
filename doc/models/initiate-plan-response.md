
# Initiate Plan Response

## Structure

`InitiatePlanResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `InstallmentPlanNumber` | `String` | Optional | - | String getInstallmentPlanNumber() | setInstallmentPlanNumber(String installmentPlanNumber) |
| `RefOrderNumber` | `String` | Optional | - | String getRefOrderNumber() | setRefOrderNumber(String refOrderNumber) |
| `PurchaseMethod` | [`PurchaseMethodEnum`](../../doc/models/purchase-method-enum.md) | Optional | - | PurchaseMethodEnum getPurchaseMethod() | setPurchaseMethod(PurchaseMethodEnum purchaseMethod) |
| `Status` | [`PlanStatusEnum`](../../doc/models/plan-status-enum.md) | Required | - | PlanStatusEnum getStatus() | setStatus(PlanStatusEnum status) |
| `Currency` | `String` | Optional | - | String getCurrency() | setCurrency(String currency) |
| `Amount` | `Double` | Optional | - | Double getAmount() | setAmount(Double amount) |
| `ExtendedParams` | `Map<String, String>` | Optional | - | Map<String, String> getExtendedParams() | setExtendedParams(Map<String, String> extendedParams) |
| `Shopper` | [`ShopperData`](../../doc/models/shopper-data.md) | Optional | - | ShopperData getShopper() | setShopper(ShopperData shopper) |
| `BillingAddress` | [`AddressData`](../../doc/models/address-data.md) | Optional | - | AddressData getBillingAddress() | setBillingAddress(AddressData billingAddress) |
| `CheckoutUrl` | `String` | Optional | - | String getCheckoutUrl() | setCheckoutUrl(String checkoutUrl) |
| `PrincipalAmount` | `Double` | Optional | - | Double getPrincipalAmount() | setPrincipalAmount(Double principalAmount) |

## Example (as JSON)

```json
{
  "InstallmentPlanNumber": "InstallmentPlanNumber6",
  "RefOrderNumber": "RefOrderNumber6",
  "PurchaseMethod": "InStore",
  "Status": "Initialized",
  "Currency": "Currency0",
  "Amount": 69.84
}
```

