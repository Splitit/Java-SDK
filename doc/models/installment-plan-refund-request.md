
# Installment Plan Refund Request

## Structure

`InstallmentPlanRefundRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Amount` | `String` | Required | - | String getAmount() | setAmount(String amount) |
| `RefundStrategy` | [`RefundStrategyEnum`](../../doc/models/refund-strategy-enum.md) | Optional | - | RefundStrategyEnum getRefundStrategy() | setRefundStrategy(RefundStrategyEnum refundStrategy) |
| `ReferenceId` | `String` | Optional | - | String getReferenceId() | setReferenceId(String referenceId) |

## Example (as JSON)

```json
{
  "Amount": "Amount4",
  "RefundStrategy": "FutureInstallmentsNotAllowed",
  "ReferenceId": "ReferenceId0"
}
```

