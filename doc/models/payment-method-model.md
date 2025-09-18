
# Payment Method Model

## Structure

`PaymentMethodModel`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Type` | [`PaymentMethodTypeEnum`](../../doc/models/payment-method-type-enum.md) | Required | - | PaymentMethodTypeEnum getType() | setType(PaymentMethodTypeEnum type) |
| `Card` | [`CardData`](../../doc/models/card-data.md) | Optional | - | CardData getCard() | setCard(CardData card) |
| `Token` | `String` | Optional | - | String getToken() | setToken(String token) |
| `BluesnapVaultedShopperToken` | [`BluesnapVaultedShopperToken`](../../doc/models/bluesnap-vaulted-shopper-token.md) | Optional | - | BluesnapVaultedShopperToken getBluesnapVaultedShopperToken() | setBluesnapVaultedShopperToken(BluesnapVaultedShopperToken bluesnapVaultedShopperToken) |
| `MockerShopperToken` | [`MockerShopperToken`](../../doc/models/mocker-shopper-token.md) | Optional | - | MockerShopperToken getMockerShopperToken() | setMockerShopperToken(MockerShopperToken mockerShopperToken) |
| `SpreedlyToken` | [`SpreedlyToken`](../../doc/models/spreedly-token.md) | Optional | - | SpreedlyToken getSpreedlyToken() | setSpreedlyToken(SpreedlyToken spreedlyToken) |
| `CardPAR` | `String` | Optional | - | String getCardPAR() | setCardPAR(String cardPAR) |

## Example (as JSON)

```json
{
  "Type": "Card",
  "Card": null,
  "Token": "Token6",
  "BluesnapVaultedShopperToken": null,
  "MockerShopperToken": null,
  "SpreedlyToken": null
}
```

