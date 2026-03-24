# CreateExpenseDto

## Example Usage

```typescript
import { CreateExpenseDto } from "maesn/models";

let value: CreateExpenseDto = {
  id: "<id>",
  accountCode: "<value>",
  accountId: "<id>",
  accountNumber: 3580.81,
  currency: "CDF",
  customerId: "<id>",
  exchangeRate: "<value>",
  expenseLines: [],
  description: "wash suddenly phew",
  documentId: "<id>",
  journalCode: "<value>",
  ledgerName: "<value>",
  note: "<value>",
  paymentTermId: "<id>",
  paymentType: "CHECK",
  supplierId: "<id>",
  type: "EXPENSE",
  totalGrossAmount: 2142.82,
  totalNetAmount: 7932.34,
  totalTaxAmount: 1142.81,
  transactionDate: "<value>",
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `id`                                                                               | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `accountCode`                                                                      | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `accountId`                                                                        | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `accountNumber`                                                                    | *number*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `currency`                                                                         | [models.CreateExpenseDtoCurrency](../models/create-expense-dto-currency.md)        | :heavy_check_mark:                                                                 | N/A                                                                                |
| `customerId`                                                                       | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `exchangeRate`                                                                     | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `expenseLines`                                                                     | [models.ExpenseLineItem](../models/expense-line-item.md)[]                         | :heavy_check_mark:                                                                 | N/A                                                                                |
| `description`                                                                      | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `documentId`                                                                       | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `journalCode`                                                                      | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `ledgerName`                                                                       | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `note`                                                                             | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `paymentTermId`                                                                    | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `paymentType`                                                                      | [models.CreateExpenseDtoPaymentType](../models/create-expense-dto-payment-type.md) | :heavy_check_mark:                                                                 | N/A                                                                                |
| `supplierId`                                                                       | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `type`                                                                             | [models.CreateExpenseDtoType](../models/create-expense-dto-type.md)                | :heavy_check_mark:                                                                 | N/A                                                                                |
| `totalGrossAmount`                                                                 | *number*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `totalNetAmount`                                                                   | *number*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `totalTaxAmount`                                                                   | *number*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `transactionDate`                                                                  | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |