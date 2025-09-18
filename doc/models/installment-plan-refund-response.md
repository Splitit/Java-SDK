
# Installment Plan Refund Response

## Structure

`InstallmentPlanRefundResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RefundId` | `String` | Optional | - | String getRefundId() | setRefundId(String refundId) |
| `InstallmentPlanNumber` | `String` | Optional | - | String getInstallmentPlanNumber() | setInstallmentPlanNumber(String installmentPlanNumber) |
| `Currency` | `String` | Optional | - | String getCurrency() | setCurrency(String currency) |
| `NonCreditRefundAmount` | `Double` | Optional | - | Double getNonCreditRefundAmount() | setNonCreditRefundAmount(Double nonCreditRefundAmount) |
| `CreditRefundAmount` | `Double` | Optional | - | Double getCreditRefundAmount() | setCreditRefundAmount(Double creditRefundAmount) |
| `Summary` | [`RefundSummary`](../../doc/models/refund-summary.md) | Optional | - | RefundSummary getSummary() | setSummary(RefundSummary summary) |
| `ReferenceId` | `String` | Optional | - | String getReferenceId() | setReferenceId(String referenceId) |

## Example (as JSON)

```json
{
  "RefundId": "RefundId8",
  "InstallmentPlanNumber": "InstallmentPlanNumber6",
  "Currency": "Currency0",
  "NonCreditRefundAmount": 1.76,
  "CreditRefundAmount": 182.3
}
```

