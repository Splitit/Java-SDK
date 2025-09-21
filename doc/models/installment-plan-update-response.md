
# Installment Plan Update Response

## Structure

`InstallmentPlanUpdateResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RefOrderNumber` | `String` | Optional | - | String getRefOrderNumber() | setRefOrderNumber(String refOrderNumber) |
| `InstallmentPlanNumber` | `String` | Optional | - | String getInstallmentPlanNumber() | setInstallmentPlanNumber(String installmentPlanNumber) |
| `Status` | [`PlanStatusEnum`](../../doc/models/plan-status-enum.md) | Required | - | PlanStatusEnum getStatus() | setStatus(PlanStatusEnum status) |
| `ShippingStatus` | [`ShippingStatusEnum`](../../doc/models/shipping-status-enum.md) | Required | - | ShippingStatusEnum getShippingStatus() | setShippingStatus(ShippingStatusEnum shippingStatus) |
| `NewAmount` | `Double` | Optional | - | Double getNewAmount() | setNewAmount(Double newAmount) |

## Example (as JSON)

```json
{
  "RefOrderNumber": "RefOrderNumber2",
  "InstallmentPlanNumber": "InstallmentPlanNumber2",
  "Status": "PendingCapture",
  "ShippingStatus": "Delivered",
  "NewAmount": 233.54
}
```

