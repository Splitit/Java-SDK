
# Card Data

## Structure

`CardData`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `CardHolderFullName` | `String` | Optional | - | String getCardHolderFullName() | setCardHolderFullName(String cardHolderFullName) |
| `CardNumber` | `String` | Optional | - | String getCardNumber() | setCardNumber(String cardNumber) |
| `CardExpYear` | `String` | Optional | - | String getCardExpYear() | setCardExpYear(String cardExpYear) |
| `CardExpMonth` | `String` | Optional | - | String getCardExpMonth() | setCardExpMonth(String cardExpMonth) |
| `CardCvv` | `String` | Optional | - | String getCardCvv() | setCardCvv(String cardCvv) |
| `CardBrand` | [`CardBrandEnum`](../../doc/models/card-brand-enum.md) | Optional | - | CardBrandEnum getCardBrand() | setCardBrand(CardBrandEnum cardBrand) |
| `CardType` | [`CardTypeEnum`](../../doc/models/card-type-enum.md) | Optional | - | CardTypeEnum getCardType() | setCardType(CardTypeEnum cardType) |

## Example (as JSON)

```json
{
  "CardHolderFullName": "CardHolderFullName8",
  "CardNumber": "CardNumber2",
  "CardExpYear": "CardExpYear4",
  "CardExpMonth": "CardExpMonth0",
  "CardCvv": "CardCvv8"
}
```

