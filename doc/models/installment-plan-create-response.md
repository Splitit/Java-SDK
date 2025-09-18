
# Installment Plan Create Response

## Structure

`InstallmentPlanCreateResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `InstallmentPlanNumber` | `String` | Optional | - | String getInstallmentPlanNumber() | setInstallmentPlanNumber(String installmentPlanNumber) |
| `DateCreated` | `LocalDateTime` | Required | - | LocalDateTime getDateCreated() | setDateCreated(LocalDateTime dateCreated) |
| `RefOrderNumber` | `String` | Optional | - | String getRefOrderNumber() | setRefOrderNumber(String refOrderNumber) |
| `PurchaseMethod` | [`PurchaseMethodEnum`](../../doc/models/purchase-method-enum.md) | Optional | - | PurchaseMethodEnum getPurchaseMethod() | setPurchaseMethod(PurchaseMethodEnum purchaseMethod) |
| `Status` | [`PlanStatusEnum`](../../doc/models/plan-status-enum.md) | Required | - | PlanStatusEnum getStatus() | setStatus(PlanStatusEnum status) |
| `Currency` | `String` | Optional | - | String getCurrency() | setCurrency(String currency) |
| `OriginalAmount` | `Double` | Optional | - | Double getOriginalAmount() | setOriginalAmount(Double originalAmount) |
| `Amount` | `Double` | Optional | - | Double getAmount() | setAmount(Double amount) |
| `ExtendedParams` | `Map<String, String>` | Optional | - | Map<String, String> getExtendedParams() | setExtendedParams(Map<String, String> extendedParams) |
| `Authorization` | [`AuthorizationModel`](../../doc/models/authorization-model.md) | Optional | - | AuthorizationModel getAuthorization() | setAuthorization(AuthorizationModel authorization) |
| `Shopper` | [`ShopperData`](../../doc/models/shopper-data.md) | Optional | - | ShopperData getShopper() | setShopper(ShopperData shopper) |
| `BillingAddress` | [`AddressData`](../../doc/models/address-data.md) | Optional | - | AddressData getBillingAddress() | setBillingAddress(AddressData billingAddress) |
| `PaymentMethod` | [`PaymentMethodModel`](../../doc/models/payment-method-model.md) | Optional | - | PaymentMethodModel getPaymentMethod() | setPaymentMethod(PaymentMethodModel paymentMethod) |
| `Installments` | [`List<Installment>`](../../doc/models/installment.md) | Optional | - | List<Installment> getInstallments() | setInstallments(List<Installment> installments) |
| `Links` | [`LinksData`](../../doc/models/links-data.md) | Optional | - | LinksData getLinks() | setLinks(LinksData links) |

## Example (as JSON)

```json
{
  "InstallmentPlanNumber": "InstallmentPlanNumber4",
  "DateCreated": "2016-03-13T12:52:32.123Z",
  "RefOrderNumber": "RefOrderNumber4",
  "PurchaseMethod": "InStore",
  "Status": "Cleared",
  "Currency": "Currency8",
  "OriginalAmount": 3.8
}
```

