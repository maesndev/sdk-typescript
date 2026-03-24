# CreateBankAccountRequestDto

## Example Usage

```typescript
import { CreateBankAccountRequestDto } from "maesn/models";

let value: CreateBankAccountRequestDto = {
  balance: 1980.04,
  bankName: "<value>",
  bic: "<value>",
  currency: "HKD",
  description: "whoa competent hopelessly provided",
  fileType: "MT940",
  iban: "RS85177400240170706062",
  name: "<value>",
  number: "<value>",
  system: "<value>",
  status: "ACTIVE",
  type: "COST",
};
```

## Fields

| Field                                                                                                | Type                                                                                                 | Required                                                                                             | Description                                                                                          |
| ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| `balance`                                                                                            | *number*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `bankName`                                                                                           | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `bic`                                                                                                | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `currency`                                                                                           | [models.CreateBankAccountRequestDtoCurrency](../models/create-bank-account-request-dto-currency.md)  | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `description`                                                                                        | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `fileType`                                                                                           | [models.CreateBankAccountRequestDtoFileType](../models/create-bank-account-request-dto-file-type.md) | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `iban`                                                                                               | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `name`                                                                                               | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `number`                                                                                             | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `system`                                                                                             | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `status`                                                                                             | [models.CreateBankAccountRequestDtoStatus](../models/create-bank-account-request-dto-status.md)      | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `type`                                                                                               | [models.CreateBankAccountRequestDtoType](../models/create-bank-account-request-dto-type.md)          | :heavy_check_mark:                                                                                   | N/A                                                                                                  |