# GetExpenseResponse

Expense record matching the provided ID

## Example Usage

```typescript
import { GetExpenseResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetExpenseResponse = {
  data: {
    id: "<id>",
    accountCode: "<value>",
    accountId: "<id>",
    accountNumber: 2055.72,
    createdDate: "<value>",
    currency: "JOD",
    customerId: "<id>",
    description: "astride what whether innocent reckless near mmm versus",
    documentId: "<id>",
    exchangeRate: "<value>",
    expenseLines: [],
    files: [
      "<value 1>",
      "<value 2>",
      "<value 3>",
    ],
    journalCode: "<value>",
    ledgerName: null,
    note: "<value>",
    paymentTermId: null,
    paymentType: "CREDIT",
    supplierId: "<id>",
    taskId: "<id>",
    type: "REFUND",
    totalGrossAmount: 1789.38,
    totalNetAmount: 5283.48,
    totalTaxAmount: 6721.36,
    transactionDate: "<value>",
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `meta`                                                                          | [operations.GetExpenseMeta](../../models/operations/get-expense-meta.md)        | :heavy_minus_sign:                                                              | N/A                                                                             |
| `data`                                                                          | [models.ExpenseResponseDto](../../models/expense-response-dto.md)               | :heavy_check_mark:                                                              | N/A                                                                             |
| `errors`                                                                        | [operations.GetExpenseErrors](../../models/operations/get-expense-errors.md)    | :heavy_check_mark:                                                              | N/A                                                                             |
| `rawData`                                                                       | [operations.GetExpenseRawData](../../models/operations/get-expense-raw-data.md) | :heavy_check_mark:                                                              | N/A                                                                             |