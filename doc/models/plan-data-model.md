
# Plan Data Model

## Structure

`PlanDataModel`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TotalAmount` | `String` | Required | - | String getTotalAmount() | setTotalAmount(String totalAmount) |
| `Currency` | `String` | Optional | - | String getCurrency() | setCurrency(String currency) |
| `NumberOfInstallments` | `Integer` | Optional | - | Integer getNumberOfInstallments() | setNumberOfInstallments(Integer numberOfInstallments) |
| `TerminalId` | `String` | Optional | - | String getTerminalId() | setTerminalId(String terminalId) |
| `PurchaseMethod` | [`PurchaseMethodEnum`](../../doc/models/purchase-method-enum.md) | Required | - | PurchaseMethodEnum getPurchaseMethod() | setPurchaseMethod(PurchaseMethodEnum purchaseMethod) |
| `RefOrderNumber` | `String` | Optional | - | String getRefOrderNumber() | setRefOrderNumber(String refOrderNumber) |
| `ExtendedParams` | `Map<String, String>` | Optional | - | Map<String, String> getExtendedParams() | setExtendedParams(Map<String, String> extendedParams) |
| `FirstInstallmentAmount` | `String` | Optional | - | String getFirstInstallmentAmount() | setFirstInstallmentAmount(String firstInstallmentAmount) |
| `FirstInstallmentDate` | `LocalDateTime` | Optional | - | LocalDateTime getFirstInstallmentDate() | setFirstInstallmentDate(LocalDateTime firstInstallmentDate) |

## Example (as JSON)

```json
{
  "TotalAmount": "TotalAmount4",
  "Currency": "Currency6",
  "NumberOfInstallments": 154,
  "TerminalId": "TerminalId8",
  "PurchaseMethod": "ECommerce",
  "RefOrderNumber": "RefOrderNumber2",
  "ExtendedParams": {
    "key0": "ExtendedParams6",
    "key1": "ExtendedParams5",
    "key2": "ExtendedParams4"
  }
}
```

