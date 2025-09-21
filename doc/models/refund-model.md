
# Refund Model

## Structure

`RefundModel`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RefundId` | `String` | Optional | - | String getRefundId() | setRefundId(String refundId) |
| `SubmitDate` | `LocalDateTime` | Required | - | LocalDateTime getSubmitDate() | setSubmitDate(LocalDateTime submitDate) |
| `TotalAmount` | `double` | Required | - | double getTotalAmount() | setTotalAmount(double totalAmount) |
| `Status` | [`RefundStatusEnum`](../../doc/models/refund-status-enum.md) | Required | - | RefundStatusEnum getStatus() | setStatus(RefundStatusEnum status) |
| `NonCreditRefundAmount` | `double` | Required | - | double getNonCreditRefundAmount() | setNonCreditRefundAmount(double nonCreditRefundAmount) |
| `CreditRefundAmount` | `double` | Required | - | double getCreditRefundAmount() | setCreditRefundAmount(double creditRefundAmount) |
| `ReferenceId` | `String` | Optional | - | String getReferenceId() | setReferenceId(String referenceId) |

## Example (as JSON)

```json
{
  "RefundId": "RefundId0",
  "SubmitDate": "2016-03-13T12:52:32.123Z",
  "TotalAmount": 115.92,
  "Status": "Pending",
  "NonCreditRefundAmount": 172.08,
  "CreditRefundAmount": 159.38,
  "ReferenceId": "ReferenceId8"
}
```

