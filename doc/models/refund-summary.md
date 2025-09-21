
# Refund Summary

## Structure

`RefundSummary`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TotalAmount` | `Double` | Optional | - | Double getTotalAmount() | setTotalAmount(Double totalAmount) |
| `FailedAmount` | `Double` | Optional | - | Double getFailedAmount() | setFailedAmount(Double failedAmount) |
| `SucceededAmount` | `Double` | Optional | - | Double getSucceededAmount() | setSucceededAmount(Double succeededAmount) |
| `PendingAmount` | `Double` | Optional | - | Double getPendingAmount() | setPendingAmount(Double pendingAmount) |

## Example (as JSON)

```json
{
  "TotalAmount": 115.98,
  "FailedAmount": 192.04,
  "SucceededAmount": 243.84,
  "PendingAmount": 20.8
}
```

