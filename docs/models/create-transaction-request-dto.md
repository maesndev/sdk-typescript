# CreateTransactionRequestDto

## Example Usage

```typescript
import { CreateTransactionRequestDto } from "maesn/models";

let value: CreateTransactionRequestDto = {
  id: "<id>",
  accountId: "<id>",
  accountNumber: 4761.77,
  amount: 1373.2,
  bookingDate: "<value>",
  code: "<value>",
  contact: "<value>",
  currency: "QAR",
  description: "commonly outside pace pleasant well-off",
  journalCode: "<value>",
  ledgerName: "<value>",
  reference: "<value>",
  status: "PRIVATE",
  taxRatePercentage: 5236.16,
  type: "SPEND",
  valueDate: "<value>",
};
```

## Fields

| Field                                                                                              | Type                                                                                               | Required                                                                                           | Description                                                                                        |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| `id`                                                                                               | *string*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `accountId`                                                                                        | *string*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `accountNumber`                                                                                    | *number*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `amount`                                                                                           | *number*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `bookingDate`                                                                                      | *string*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `code`                                                                                             | *string*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `contact`                                                                                          | *string*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `currency`                                                                                         | [models.CreateTransactionRequestDtoCurrency](../models/create-transaction-request-dto-currency.md) | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `description`                                                                                      | *string*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `journalCode`                                                                                      | *string*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `ledgerName`                                                                                       | *string*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `reference`                                                                                        | *string*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `status`                                                                                           | [models.CreateTransactionRequestDtoStatus](../models/create-transaction-request-dto-status.md)     | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `taxRatePercentage`                                                                                | *number*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `type`                                                                                             | [models.CreateTransactionRequestDtoType](../models/create-transaction-request-dto-type.md)         | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `valueDate`                                                                                        | *string*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |