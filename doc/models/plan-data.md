
# Plan Data

## Structure

`PlanData`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TerminalId` | `String` | Optional | - | String getTerminalId() | setTerminalId(String terminalId) |
| `TotalAmount` | `String` | Required | - | String getTotalAmount() | setTotalAmount(String totalAmount) |
| `FirstInstallmentAmount` | `Double` | Optional | - | Double getFirstInstallmentAmount() | setFirstInstallmentAmount(Double firstInstallmentAmount) |
| `Currency` | `String` | Optional | - | String getCurrency() | setCurrency(String currency) |
| `NumberOfInstallments` | `int` | Required | - | int getNumberOfInstallments() | setNumberOfInstallments(int numberOfInstallments) |
| `PurchaseMethod` | [`PurchaseMethodEnum`](../../doc/models/purchase-method-enum.md) | Required | - | PurchaseMethodEnum getPurchaseMethod() | setPurchaseMethod(PurchaseMethodEnum purchaseMethod) |
| `RefOrderNumber` | `String` | Optional | - | String getRefOrderNumber() | setRefOrderNumber(String refOrderNumber) |
| `AllowedInstallmentOptions` | `List<Integer>` | Optional | - | List<Integer> getAllowedInstallmentOptions() | setAllowedInstallmentOptions(List<Integer> allowedInstallmentOptions) |
| `Tags` | `Map<String, String>` | Optional | - | Map<String, String> getTags() | setTags(Map<String, String> tags) |
| `ProcessingData` | [`ProcessingData`](../../doc/models/processing-data.md) | Optional | - | ProcessingData getProcessingData() | setProcessingData(ProcessingData processingData) |
| `FirstInstallmentDate` | `LocalDateTime` | Optional | - | LocalDateTime getFirstInstallmentDate() | setFirstInstallmentDate(LocalDateTime firstInstallmentDate) |

## Example (as JSON)

```json
{
  "TerminalId": "TerminalId8",
  "TotalAmount": "TotalAmount4",
  "FirstInstallmentAmount": 11.28,
  "Currency": "Currency6",
  "NumberOfInstallments": 2,
  "PurchaseMethod": "PhoneOrder",
  "RefOrderNumber": "RefOrderNumber2",
  "AllowedInstallmentOptions": [
    46,
    47
  ]
}
```

