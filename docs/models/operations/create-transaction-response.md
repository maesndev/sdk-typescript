# CreateTransactionResponse

Transaction created successfully

## Example Usage

```typescript
import { CreateTransactionResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateTransactionResponse = {
  data: {
    id: "<id>",
    accountId: "<id>",
    accountNumber: 1003,
    amount: 713.23,
    bookingDate: "<value>",
    contact: "<value>",
    currency: "USD",
    description:
      "joyous forecast speedily selfishly that apropos obtrude receptor",
    files: [
      "<value 1>",
    ],
    journalCode: "<value>",
    ledgerName: "<value>",
    reference: null,
    status: "PRIVATE",
    taskId: "<id>",
    taxRatePercentage: 7224.28,
    type: "SPEND-TRANSFER",
    valueDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `meta`                                                                                        | [operations.CreateTransactionMeta](../../models/operations/create-transaction-meta.md)        | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `data`                                                                                        | [models.TransactionResponseDto](../../models/transaction-response-dto.md)                     | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `errors`                                                                                      | [operations.CreateTransactionErrors](../../models/operations/create-transaction-errors.md)    | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `rawData`                                                                                     | [operations.CreateTransactionRawData](../../models/operations/create-transaction-raw-data.md) | :heavy_check_mark:                                                                            | N/A                                                                                           |