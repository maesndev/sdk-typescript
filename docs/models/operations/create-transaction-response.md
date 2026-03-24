# CreateTransactionResponse

## Example Usage

```typescript
import { CreateTransactionResponse } from "maesn/models/operations";

let value: CreateTransactionResponse = {
  meta: {
    warnings: [
      "<value 1>",
      "<value 2>",
    ],
    pagination: {
      total: 3438.77,
      perPage: 5109.63,
      currentPage: 2626.79,
      totalPages: 3561.84,
    },
  },
  data: {
    id: "<id>",
    accountId: "<id>",
    accountNumber: 3775.52,
    amount: 8741.3,
    bookingDate: "<value>",
    contact: "<value>",
    currency: "KES",
    description: "as outlying when",
    files: [
      "<value 1>",
    ],
    journalCode: "<value>",
    ledgerName: "<value>",
    reference: "<value>",
    status: "BOOKED",
    taskId: "<id>",
    taxRatePercentage: 7705.57,
    type: "RECEIVE-TRANSFER",
    valueDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `meta`                                                                                        | [models.MetaResponse](../../models/meta-response.md)                                          | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `data`                                                                                        | [models.TransactionResponseDto](../../models/transaction-response-dto.md)                     | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `errors`                                                                                      | [operations.CreateTransactionErrors](../../models/operations/create-transaction-errors.md)    | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `rawData`                                                                                     | [operations.CreateTransactionRawData](../../models/operations/create-transaction-raw-data.md) | :heavy_check_mark:                                                                            | N/A                                                                                           |