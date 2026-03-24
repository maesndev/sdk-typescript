# ExpenseLineItem

## Example Usage

```typescript
import { ExpenseLineItem } from "maesn/models";

let value: ExpenseLineItem = {
  id: "<id>",
  accountCode: "<value>",
  accountId: "<id>",
  accountNumber: 7578.79,
  currency: "KPW",
  description: "fussy lobotomise plain rebuke and hence provided pack finally",
  dimensions: [
    "<value 1>",
    "<value 2>",
  ],
  documentNumber: "<value>",
  exchangeRate: 6370.59,
  itemId: "<id>",
  taxRate: {
    id: "<id>",
    code: "<value>",
    name: "<value>",
    taxRatePercentage: "<value>",
  },
  totalGrossAmount: 6102.94,
  totalNetAmount: 7148.83,
};
```

## Fields

| Field                                                                     | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `id`                                                                      | *string*                                                                  | :heavy_check_mark:                                                        | N/A                                                                       |
| `accountCode`                                                             | *string*                                                                  | :heavy_check_mark:                                                        | N/A                                                                       |
| `accountId`                                                               | *string*                                                                  | :heavy_check_mark:                                                        | N/A                                                                       |
| `accountNumber`                                                           | *number*                                                                  | :heavy_check_mark:                                                        | N/A                                                                       |
| `currency`                                                                | [models.ExpenseLineItemCurrency](../models/expense-line-item-currency.md) | :heavy_check_mark:                                                        | N/A                                                                       |
| `description`                                                             | *string*                                                                  | :heavy_check_mark:                                                        | N/A                                                                       |
| `dimensions`                                                              | *string*[]                                                                | :heavy_check_mark:                                                        | N/A                                                                       |
| `documentNumber`                                                          | *string*                                                                  | :heavy_check_mark:                                                        | N/A                                                                       |
| `exchangeRate`                                                            | *number*                                                                  | :heavy_check_mark:                                                        | N/A                                                                       |
| `itemId`                                                                  | *string*                                                                  | :heavy_check_mark:                                                        | N/A                                                                       |
| `taxRate`                                                                 | [models.TaxRate](../models/tax-rate.md)                                   | :heavy_check_mark:                                                        | N/A                                                                       |
| `totalGrossAmount`                                                        | *number*                                                                  | :heavy_check_mark:                                                        | N/A                                                                       |
| `totalNetAmount`                                                          | *number*                                                                  | :heavy_check_mark:                                                        | N/A                                                                       |