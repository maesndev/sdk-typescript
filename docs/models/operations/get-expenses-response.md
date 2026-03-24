# GetExpensesResponse

## Example Usage

```typescript
import { GetExpensesResponse } from "maesn/models/operations";

let value: GetExpensesResponse = {
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
  data: [
    {
      id: "<id>",
      accountCode: "<value>",
      accountId: "<id>",
      accountNumber: 2489.95,
      createdDate: "<value>",
      currency: "BSD",
      customerId: "<id>",
      description: "giving readmit readjust whenever till",
      documentId: "<id>",
      exchangeRate: "<value>",
      expenseLines: [],
      files: [
        "<value 1>",
      ],
      journalCode: "<value>",
      ledgerName: "<value>",
      note: "<value>",
      paymentTermId: "<id>",
      paymentType: "CREDIT_CARD",
      supplierId: "<id>",
      taskId: "<id>",
      type: "EXPENSE",
      totalGrossAmount: 2630.57,
      totalNetAmount: 8117.72,
      totalTaxAmount: 811.76,
      transactionDate: "<value>",
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `meta`                                                                            | [models.MetaResponse](../../models/meta-response.md)                              | :heavy_check_mark:                                                                | N/A                                                                               |
| `data`                                                                            | [models.ExpenseResponseDto](../../models/expense-response-dto.md)[]               | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetExpensesErrors](../../models/operations/get-expenses-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetExpensesRawData](../../models/operations/get-expenses-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |