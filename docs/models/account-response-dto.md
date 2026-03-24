# AccountResponseDto

## Example Usage

```typescript
import { AccountResponseDto } from "maesn/models";

let value: AccountResponseDto = {
  id: "<id>",
  balance: 1988.39,
  class: "REVENUE",
  code: "<value>",
  createdDate: "<value>",
  currency: "CDF",
  debitCreditIndicator: "DEBIT",
  description: "drat jungle so intent except",
  name: "<value>",
  number: "<value>",
  parentAccountId: "<id>",
  status: "ACTIVE",
  type: "<value>",
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                                     | Type                                                                                                      | Required                                                                                                  | Description                                                                                               |
| --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                      | *string*                                                                                                  | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `balance`                                                                                                 | *number*                                                                                                  | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `class`                                                                                                   | [models.AccountResponseDtoClass](../models/account-response-dto-class.md)                                 | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `code`                                                                                                    | *string*                                                                                                  | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `createdDate`                                                                                             | *string*                                                                                                  | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `currency`                                                                                                | [models.AccountResponseDtoCurrency](../models/account-response-dto-currency.md)                           | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `debitCreditIndicator`                                                                                    | [models.AccountResponseDtoDebitCreditIndicator](../models/account-response-dto-debit-credit-indicator.md) | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `description`                                                                                             | *string*                                                                                                  | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `name`                                                                                                    | *string*                                                                                                  | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `number`                                                                                                  | *string*                                                                                                  | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `parentAccountId`                                                                                         | *string*                                                                                                  | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `status`                                                                                                  | [models.AccountResponseDtoStatus](../models/account-response-dto-status.md)                               | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `type`                                                                                                    | *string*                                                                                                  | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `updatedDate`                                                                                             | *string*                                                                                                  | :heavy_check_mark:                                                                                        | N/A                                                                                                       |