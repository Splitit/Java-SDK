
# Installments Eligibility Response

## Structure

`InstallmentsEligibilityResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `InstallmentProvider` | `String` | Optional | - | String getInstallmentProvider() | setInstallmentProvider(String installmentProvider) |
| `PaymentPlanOptions` | [`List<PaymentPlanOptionModel>`](../../doc/models/payment-plan-option-model.md) | Optional | - | List<PaymentPlanOptionModel> getPaymentPlanOptions() | setPaymentPlanOptions(List<PaymentPlanOptionModel> paymentPlanOptions) |

## Example (as JSON)

```json
{
  "InstallmentProvider": "InstallmentProvider2",
  "PaymentPlanOptions": [
    null,
    {},
    {}
  ]
}
```

