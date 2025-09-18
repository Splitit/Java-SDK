
# Plan Error Response Exception

## Structure

`PlanErrorResponseException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TraceId` | `String` | Optional | - | String getTraceId() | setTraceId(String traceId) |
| `Error` | [`ErrorExtended`](../../doc/models/error-extended.md) | Optional | - | ErrorExtended getError() | setError(ErrorExtended error) |
| `InstallmentPlanNumber` | `String` | Optional | - | String getInstallmentPlanNumber() | setInstallmentPlanNumber(String installmentPlanNumber) |
| `PaymentInfo` | [`PaymentInfo`](../../doc/models/payment-info.md) | Optional | - | PaymentInfo getPaymentInfo() | setPaymentInfo(PaymentInfo paymentInfo) |

## Example (as JSON)

```json
{
  "TraceId": "TraceId8",
  "Error": null,
  "InstallmentPlanNumber": "InstallmentPlanNumber6",
  "PaymentInfo": null
}
```

