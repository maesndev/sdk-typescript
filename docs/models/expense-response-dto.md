# ExpenseResponseDto

## Example Usage

```typescript
import { ExpenseResponseDto } from "@maesn/typescript-sdk/models";

let value: ExpenseResponseDto = {
  id: "<id>",
  accountCode: "<value>",
  accountId: "<id>",
  accountNumber: 1972.27,
  createdDate: "<value>",
  currency: "GTQ",
  customerId: "<id>",
  description: "boldly broadly parched",
  documentId: "<id>",
  exchangeRate: null,
  expenseLines: [
    {
      id: "<id>",
      accountCode: "<value>",
      accountId: "<id>",
      accountNumber: 8184.99,
      createdDate: "<value>",
      currency: "CRC",
      description:
        "however airline bran briskly elegant micromanage gazebo upbeat morning",
      dimensions: [
        {
          id: "<id>",
          categoryName: "<value>",
          name: "<value>",
        },
      ],
      documentNumber: "<value>",
      exchangeRate: 5986.84,
      itemId: "<id>",
      taxRate: {
        id: "<id>",
        code: "<value>",
        name: null,
        taxRatePercentage: "<value>",
      },
      totalGrossAmount: 2525.53,
      totalNetAmount: 5320.75,
      updatedDate: "<value>",
    },
  ],
  files: [
    "<value 1>",
  ],
  journalCode: "<value>",
  ledgerName: "<value>",
  note: "<value>",
  paymentTermId: "<id>",
  paymentType: null,
  supplierId: "<id>",
  taskId: "<id>",
  type: "EXPENSE",
  totalGrossAmount: 6948.88,
  totalNetAmount: null,
  totalTaxAmount: 3254.09,
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