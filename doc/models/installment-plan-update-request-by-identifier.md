
# Installment Plan Update Request by Identifier

## Structure

`InstallmentPlanUpdateRequestByIdentifier`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RefOrderNumber` | `String` | Optional | - | String getRefOrderNumber() | setRefOrderNumber(String refOrderNumber) |
| `TrackingNumber` | `String` | Optional | - | String getTrackingNumber() | setTrackingNumber(String trackingNumber) |
| `Capture` | `Boolean` | Optional | - | Boolean getCapture() | setCapture(Boolean capture) |
| `ShippingStatus` | [`ShippingStatusEnum`](../../doc/models/shipping-status-enum.md) | Optional | - | ShippingStatusEnum getShippingStatus() | setShippingStatus(ShippingStatusEnum shippingStatus) |
| `NewAmount` | `Double` | Optional | - | Double getNewAmount() | setNewAmount(Double newAmount) |
| `Identifier` | [`IdentifierContract`](../../doc/models/identifier-contract.md) | Optional | - | IdentifierContract getIdentifier() | setIdentifier(IdentifierContract identifier) |

## Example (as JSON)

```json
{
  "RefOrderNumber": "RefOrderNumber2",
  "TrackingNumber": "TrackingNumber6",
  "Capture": false,
  "ShippingStatus": "Pending",
  "NewAmount": 233.74
}
```

