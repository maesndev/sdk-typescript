# BankAccountResponseDto

## Example Usage

```typescript
import { BankAccountResponseDto } from "maesn/models";

let value: BankAccountResponseDto = {
  id: "<id>",
  balance: 7843.73,
  bankName: "<value>",
  bic: "<value>",
  createdDate: "<value>",
  currency: "JPY",
  description: "boohoo ouch vice not upright overspend what",
  fileType: "CSV",
  iban: "LI2002338T9839241M532",
  name: "<value>",
  number: "<value>",
  system: "<value>",
  status: "ACTIVE",
  type: "<value>",
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                     | Type                                                                                      | Required                                                                                  | Description                                                                               |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `id`                                                                                      | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `balance`                                                                                 | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `bankName`                                                                                | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `bic`                                                                                     | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `createdDate`                                                                             | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `currency`                                                                                | [models.BankAccountResponseDtoCurrency](../models/bank-account-response-dto-currency.md)  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `description`                                                                             | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `fileType`                                                                                | [models.BankAccountResponseDtoFileType](../models/bank-account-response-dto-file-type.md) | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `iban`                                                                                    | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `name`                                                                                    | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `number`                                                                                  | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `system`                                                                                  | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `status`                                                                                  | [models.BankAccountResponseDtoStatus](../models/bank-account-response-dto-status.md)      | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `type`                                                                                    | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `updatedDate`                                                                             | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |