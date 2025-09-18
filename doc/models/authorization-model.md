
# Authorization Model

## Structure

`AuthorizationModel`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Status` | [`GwAuthorizationStatusEnum`](../../doc/models/gw-authorization-status-enum.md) | Required | - | GwAuthorizationStatusEnum getStatus() | setStatus(GwAuthorizationStatusEnum status) |
| `Date` | `LocalDateTime` | Optional | - | LocalDateTime getDate() | setDate(LocalDateTime date) |
| `SplititErrorResultCode` | `String` | Optional | - | String getSplititErrorResultCode() | setSplititErrorResultCode(String splititErrorResultCode) |
| `GatewayTransactionID` | `String` | Optional | - | String getGatewayTransactionID() | setGatewayTransactionID(String gatewayTransactionID) |
| `GatewayResultCode` | `String` | Optional | - | String getGatewayResultCode() | setGatewayResultCode(String gatewayResultCode) |
| `GatewayResultMessage` | `String` | Optional | - | String getGatewayResultMessage() | setGatewayResultMessage(String gatewayResultMessage) |
| `ThreeDSRedirect` | [`ThreeDsRedirectDataV3`](../../doc/models/three-ds-redirect-data-v3.md) | Optional | - | ThreeDsRedirectDataV3 getThreeDSRedirect() | setThreeDSRedirect(ThreeDsRedirectDataV3 threeDSRedirect) |
| `CAVV` | `String` | Optional | - | String getCAVV() | setCAVV(String cAVV) |
| `ECI` | `String` | Optional | - | String getECI() | setECI(String eCI) |
| `GatewaySourceResponse` | `String` | Optional | - | String getGatewaySourceResponse() | setGatewaySourceResponse(String gatewaySourceResponse) |

## Example (as JSON)

```json
{
  "Status": "Canceled",
  "Date": "2016-03-13T12:52:32.123Z",
  "SplititErrorResultCode": "SplititErrorResultCode6",
  "GatewayTransactionID": "GatewayTransactionID0",
  "GatewayResultCode": "GatewayResultCode2",
  "GatewayResultMessage": "GatewayResultMessage8"
}
```

