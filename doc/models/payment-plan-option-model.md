
# Payment Plan Option Model

## Structure

`PaymentPlanOptionModel`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `NumberOfInstallments` | `int` | Required | - | int getNumberOfInstallments() | setNumberOfInstallments(int numberOfInstallments) |
| `FirstInstallmentAmount` | `double` | Required | - | double getFirstInstallmentAmount() | setFirstInstallmentAmount(double firstInstallmentAmount) |
| `InstallmentAmount` | `double` | Required | - | double getInstallmentAmount() | setInstallmentAmount(double installmentAmount) |
| `LastInstallmentAmount` | `double` | Required | - | double getLastInstallmentAmount() | setLastInstallmentAmount(double lastInstallmentAmount) |
| `Links` | [`LinksModel`](../../doc/models/links-model.md) | Optional | - | LinksModel getLinks() | setLinks(LinksModel links) |
| `TermsAndConditionsBrief` | `String` | Optional | - | String getTermsAndConditionsBrief() | setTermsAndConditionsBrief(String termsAndConditionsBrief) |
| `InstallmentFrequency` | `String` | Optional | - | String getInstallmentFrequency() | setInstallmentFrequency(String installmentFrequency) |

## Example (as JSON)

```json
{
  "NumberOfInstallments": 148,
  "FirstInstallmentAmount": 45.62,
  "InstallmentAmount": 232.3,
  "LastInstallmentAmount": 187.9,
  "Links": null,
  "TermsAndConditionsBrief": "TermsAndConditionsBrief6",
  "InstallmentFrequency": "InstallmentFrequency2"
}
```

