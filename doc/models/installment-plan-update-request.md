
# Installment Plan Update Request

## Structure

`InstallmentPlanUpdateRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RefOrderNumber` | `String` | Optional | - | String getRefOrderNumber() | setRefOrderNumber(String refOrderNumber) |
| `TrackingNumber` | `String` | Optional | - | String getTrackingNumber() | setTrackingNumber(String trackingNumber) |
| `Capture` | `Boolean` | Optional | - | Boolean getCapture() | setCapture(Boolean capture) |
| `ShippingStatus` | [`ShippingStatusEnum`](../../doc/models/shipping-status-enum.md) | Optional | - | ShippingStatusEnum getShippingStatus() | setShippingStatus(ShippingStatusEnum shippingStatus) |
| `NewAmount` | `String` | Optional | - | String getNewAmount() | setNewAmount(String newAmount) |

## Example (as JSON)

```json
{
  "RefOrderNumber": "RefOrderNumber2",
  "TrackingNumber": "TrackingNumber6",
  "Capture": false,
  "ShippingStatus": "Shipped",
  "NewAmount": "NewAmount4"
}
```

