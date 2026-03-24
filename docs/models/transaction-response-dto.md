# TransactionResponseDto

## Example Usage

```typescript
import { TransactionResponseDto } from "maesn/models";

let value: TransactionResponseDto = {
  id: "<id>",
  accountId: "<id>",
  accountNumber: 3055.87,
  amount: 6104.52,
  bookingDate: "<value>",
  contact: "<value>",
  currency: "BHD",
  description: "unzip once junior amazing",
  files: [],
  journalCode: "<value>",
  ledgerName: "<value>",
  reference: "<value>",
  status: "DELETED",
  taskId: "<id>",
  taxRatePercentage: 2835.14,
  type: "RECEIVE-OVERPAYMENT",
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