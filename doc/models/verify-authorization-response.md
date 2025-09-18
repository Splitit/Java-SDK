
# Verify Authorization Response

## Structure

`VerifyAuthorizationResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `IsAuthorized` | `boolean` | Required | - | boolean getIsAuthorized() | setIsAuthorized(boolean isAuthorized) |
| `AuthorizationAmount` | `Double` | Optional | - | Double getAuthorizationAmount() | setAuthorizationAmount(Double authorizationAmount) |
| `Authorization` | [`AuthorizationModel`](../../doc/models/authorization-model.md) | Optional | - | AuthorizationModel getAuthorization() | setAuthorization(AuthorizationModel authorization) |

## Example (as JSON)

```json
{
  "IsAuthorized": false,
  "AuthorizationAmount": 186.44,
  "Authorization": null
}
```

