
# Identifier Contract

## Structure

`IdentifierContract`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RefOrderNumber` | `String` | Optional | - | String getRefOrderNumber() | setRefOrderNumber(String refOrderNumber) |
| `InstallmentPlanNumber` | `String` | Optional | - | String getInstallmentPlanNumber() | setInstallmentPlanNumber(String installmentPlanNumber) |
| `ExtendedParams` | `Map<String, String>` | Optional | - | Map<String, String> getExtendedParams() | setExtendedParams(Map<String, String> extendedParams) |

## Example (as JSON)

```json
{
  "RefOrderNumber": "RefOrderNumber6",
  "InstallmentPlanNumber": "InstallmentPlanNumber6",
  "ExtendedParams": {
    "key0": "ExtendedParams6",
    "key1": "ExtendedParams7"
  }
}
```

