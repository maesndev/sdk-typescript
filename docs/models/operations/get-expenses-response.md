# GetExpensesResponse

List of expenses for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetExpensesResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetExpensesResponse = {
  data: [
    {
      id: "<id>",
      accountCode: "<value>",
      accountId: "<id>",
      accountNumber: 9900.41,
      createdDate: "<value>",
      currency: "LVL",
      customerId: "<id>",
      description:
        "realistic scientific gah drat pish exacerbate woot denitrify",
      documentId: "<id>",
      exchangeRate: "<value>",
      expenseLines: [],
      files: [],
      journalCode: null,
      ledgerName: "<value>",
      note: "<value>",
      paymentTermId: "<id>",
      paymentType: "COLLECTION",
      supplierId: "<id>",
      taskId: "<id>",
      type: null,
      totalGrossAmount: 487.12,
      totalNetAmount: null,
      totalTaxAmount: null,
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
| `meta`                                                                            | [operations.GetExpensesMeta](../../models/operations/get-expenses-meta.md)        | :heavy_minus_sign:                                                                | N/A                                                                               |
| `data`                                                                            | [models.ExpenseResponseDto](../../models/expense-response-dto.md)[]               | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetExpensesErrors](../../models/operations/get-expenses-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetExpensesRawData](../../models/operations/get-expenses-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |