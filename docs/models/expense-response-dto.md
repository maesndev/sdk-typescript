# ExpenseResponseDto

## Example Usage

```typescript
import { ExpenseResponseDto } from "maesn/models";

let value: ExpenseResponseDto = {
  id: "<id>",
  accountCode: "<value>",
  accountId: "<id>",
  accountNumber: 6832.39,
  createdDate: "<value>",
  currency: "MUR",
  customerId: "<id>",
  description: "than yahoo ignorance silt dimly ugh abnormally likewise more",
  documentId: "<id>",
  exchangeRate: "<value>",
  expenseLines: [],
  files: [],
  journalCode: "<value>",
  ledgerName: "<value>",
  note: "<value>",
  paymentTermId: "<id>",
  paymentType: "CREDIT",
  supplierId: "<id>",
  taskId: "<id>",
  type: "EXPENSE",
  totalGrossAmount: 7223.55,
  totalNetAmount: 9831.61,
  totalTaxAmount: 574.1,
  transactionDate: "<value>",
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `id`                                                                                   | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `accountCode`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `accountId`                                                                            | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `accountNumber`                                                                        | *number*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `createdDate`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `currency`                                                                             | [models.ExpenseResponseDtoCurrency](../models/expense-response-dto-currency.md)        | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `customerId`                                                                           | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `description`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `documentId`                                                                           | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `exchangeRate`                                                                         | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `expenseLines`                                                                         | [models.ExpenseLineItemResponse](../models/expense-line-item-response.md)[]            | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `files`                                                                                | *string*[]                                                                             | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `journalCode`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `ledgerName`                                                                           | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `note`                                                                                 | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `paymentTermId`                                                                        | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `paymentType`                                                                          | [models.ExpenseResponseDtoPaymentType](../models/expense-response-dto-payment-type.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `supplierId`                                                                           | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `taskId`                                                                               | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `type`                                                                                 | [models.ExpenseResponseDtoType](../models/expense-response-dto-type.md)                | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `totalGrossAmount`                                                                     | *number*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `totalNetAmount`                                                                       | *number*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `totalTaxAmount`                                                                       | *number*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `transactionDate`                                                                      | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `updatedDate`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |