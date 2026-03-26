# TransactionResponseDto

## Example Usage

```typescript
import { TransactionResponseDto } from "@maesn/typescript-sdk/models";

let value: TransactionResponseDto = {
  id: "<id>",
  accountId: "<id>",
  accountNumber: null,
  amount: 7353.2,
  bookingDate: null,
  contact: "<value>",
  currency: "GYD",
  description:
    "once junior amazing rationale in bookend whose outrank yowza reflate",
  files: [
    "<value 1>",
  ],
  journalCode: "<value>",
  ledgerName: "<value>",
  reference: "<value>",
  status: "LINKED",
  taskId: "<id>",
  taxRatePercentage: 6899.49,
  type: "RECEIVE",
  valueDate: "<value>",
};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `id`                                                                                    | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `accountId`                                                                             | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `accountNumber`                                                                         | *number*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `amount`                                                                                | *number*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `bookingDate`                                                                           | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `contact`                                                                               | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `currency`                                                                              | [models.TransactionResponseDtoCurrency](../models/transaction-response-dto-currency.md) | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `description`                                                                           | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `files`                                                                                 | *string*[]                                                                              | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `journalCode`                                                                           | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `ledgerName`                                                                            | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `reference`                                                                             | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `status`                                                                                | [models.TransactionResponseDtoStatus](../models/transaction-response-dto-status.md)     | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `taskId`                                                                                | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `taxRatePercentage`                                                                     | *number*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `type`                                                                                  | [models.TransactionResponseDtoType](../models/transaction-response-dto-type.md)         | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `valueDate`                                                                             | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |