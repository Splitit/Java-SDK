
# Installment

## Structure

`Installment`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `InstallmentNumber` | `int` | Required | - | int getInstallmentNumber() | setInstallmentNumber(int installmentNumber) |
| `Amount` | `double` | Required | - | double getAmount() | setAmount(double amount) |
| `ProcessDateTime` | `LocalDateTime` | Optional | - | LocalDateTime getProcessDateTime() | setProcessDateTime(LocalDateTime processDateTime) |
| `Status` | [`InstallmentStatusEnum`](../../doc/models/installment-status-enum.md) | Required | - | InstallmentStatusEnum getStatus() | setStatus(InstallmentStatusEnum status) |

## Example (as JSON)

```json
{
  "InstallmentNumber": 244,
  "Amount": 181.38,
  "ProcessDateTime": "2016-03-13T12:52:32.123Z",
  "Status": "Processed"
}
```

