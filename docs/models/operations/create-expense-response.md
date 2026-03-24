# CreateExpenseResponse

## Example Usage

```typescript
import { CreateExpenseResponse } from "maesn/models/operations";

let value: CreateExpenseResponse = {
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
    accountCode: "<value>",
    accountId: "<id>",
    accountNumber: 6502.37,
    createdDate: "<value>",
    currency: "NAD",
    customerId: "<id>",
    description: "fatal triumphantly anticodon aha rim via leap",
    documentId: "<id>",
    exchangeRate: "<value>",
    expenseLines: [
      {
        id: "<id>",
        accountCode: "<value>",
        accountId: "<id>",
        accountNumber: 3959.46,
        createdDate: "<value>",
        currency: "SAR",
        description:
          "bruised evil as legal factorise of while mosh hmph cleverly",
        dimensions: [
          "<value 1>",
          "<value 2>",
        ],
        documentNumber: "<value>",
        exchangeRate: 9630.37,
        itemId: "<id>",
        taxRate: {
          id: "<id>",
          code: "<value>",
          name: "<value>",
          taxRatePercentage: "<value>",
        },
        totalGrossAmount: 4109.94,
        totalNetAmount: 5817.45,
        updatedDate: "<value>",
      },
    ],
    files: [
      "<value 1>",
      "<value 2>",
    ],
    journalCode: "<value>",
    ledgerName: "<value>",
    note: "<value>",
    paymentTermId: "<id>",
    paymentType: "CHECK",
    supplierId: "<id>",
    taskId: "<id>",
    type: "REFUND",
    totalGrossAmount: 2062.55,
    totalNetAmount: 1500.58,
    totalTaxAmount: 6861.14,
    transactionDate: "<value>",
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [models.MetaResponse](../../models/meta-response.md)                                  | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `data`                                                                                | [models.ExpenseResponseDto](../../models/expense-response-dto.md)                     | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.CreateExpenseErrors](../../models/operations/create-expense-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.CreateExpenseRawData](../../models/operations/create-expense-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |