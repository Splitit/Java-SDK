
# Check Installments Eligibility Request

## Structure

`CheckInstallmentsEligibilityRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `PlanData` | [`PlanData`](../../doc/models/plan-data.md) | Optional | - | PlanData getPlanData() | setPlanData(PlanData planData) |
| `CardDetails` | [`CardData`](../../doc/models/card-data.md) | Optional | - | CardData getCardDetails() | setCardDetails(CardData cardDetails) |
| `BillingAddress` | [`AddressData`](../../doc/models/address-data.md) | Optional | - | AddressData getBillingAddress() | setBillingAddress(AddressData billingAddress) |
| `ShopperIdentifier` | `String` | Optional | - | String getShopperIdentifier() | setShopperIdentifier(String shopperIdentifier) |

## Example (as JSON)

```json
{
  "PlanData": null,
  "CardDetails": null,
  "BillingAddress": null,
  "ShopperIdentifier": "ShopperIdentifier6"
}
```

