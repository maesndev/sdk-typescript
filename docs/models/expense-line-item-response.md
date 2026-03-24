# ExpenseLineItemResponse

## Example Usage

```typescript
import { ExpenseLineItemResponse } from "maesn/models";

let value: ExpenseLineItemResponse = {
  id: "<id>",
  accountCode: "<value>",
  accountId: "<id>",
  accountNumber: 5863.22,
  createdDate: "<value>",
  currency: "CHF",
  description: "underneath by utterly where sleepily ick blah where silver",
  dimensions: [
    "<value 1>",
  ],
  documentNumber: "<value>",
  exchangeRate: 3841.29,
  itemId: "<id>",
  taxRate: {
    id: "<id>",
    code: "<value>",
    name: "<value>",
    taxRatePercentage: "<value>",
  },
  totalGrossAmount: 1185.73,
  totalNetAmount: 761.6,
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
| `dimensions`                                                                               | *string*[]                                                                                 | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `documentNumber`                                                                           | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `exchangeRate`                                                                             | *number*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `itemId`                                                                                   | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `taxRate`                                                                                  | [models.TaxRate](../models/tax-rate.md)                                                    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `totalGrossAmount`                                                                         | *number*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `totalNetAmount`                                                                           | *number*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `updatedDate`                                                                              | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |