
# Error Extended

## Structure

`ErrorExtended`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Code` | `String` | Optional | - | String getCode() | setCode(String code) |
| `Message` | `String` | Optional | - | String getMessage() | setMessage(String message) |
| `AdditionalInfo` | `String` | Optional | - | String getAdditionalInfo() | setAdditionalInfo(String additionalInfo) |
| `ExtraData` | `Map<String, String>` | Optional | - | Map<String, String> getExtraData() | setExtraData(Map<String, String> extraData) |

## Example (as JSON)

```json
{
  "Code": "Code0",
  "Message": "Message6",
  "AdditionalInfo": "AdditionalInfo8",
  "ExtraData": {
    "key0": "ExtraData0"
  }
}
```

