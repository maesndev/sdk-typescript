# ExpenseLineItemResponse

## Example Usage

```typescript
import { ExpenseLineItemResponse } from "@maesn/typescript-sdk/models";

let value: ExpenseLineItemResponse = {
  id: "<id>",
  accountCode: "<value>",
  accountId: "<id>",
  accountNumber: 1495.53,
  createdDate: "<value>",
  currency: "ZAR",
  description:
    "by utterly where sleepily ick blah where silver shrilly carpool",
  dimensions: null,
  documentNumber: "<value>",
  exchangeRate: 6736.17,
  itemId: "<id>",
  taxRate: {
    id: "<id>",
    code: "<value>",
    name: null,
    taxRatePercentage: "<value>",
  },
  totalGrossAmount: 5570.57,
  totalNetAmount: 285.5,
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `id`                                                                                       | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `accountCode`                                                                              | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `accountId`                                                                                | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `accountNumber`                                                                            | *number*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `createdDate`                                                                              | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `currency`                                                                                 | [models.ExpenseLineItemResponseCurrency](../models/expense-line-item-response-currency.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `description`                                                                              | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `dimensions`                                                                               | [models.Dimension](../models/dimension.md)[]                                               | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `documentNumber`                                                                           | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `exchangeRate`                                                                             | *number*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `itemId`                                                                                   | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `taxRate`                                                                                  | [models.ExpenseLineItemResponseTaxRate](../models/expense-line-item-response-tax-rate.md)  | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `totalGrossAmount`                                                                         | *number*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `totalNetAmount`                                                                           | *number*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `updatedDate`                                                                              | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |