# ExpenseLineItem

## Example Usage

```typescript
import { ExpenseLineItem } from "@maesn/typescript-sdk/models";

let value: ExpenseLineItem = {};
```

## Fields

| Field                                                                     | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `id`                                                                      | *string*                                                                  | :heavy_minus_sign:                                                        | N/A                                                                       |
| `accountCode`                                                             | *string*                                                                  | :heavy_minus_sign:                                                        | N/A                                                                       |
| `accountId`                                                               | *string*                                                                  | :heavy_minus_sign:                                                        | N/A                                                                       |
| `accountNumber`                                                           | *number*                                                                  | :heavy_minus_sign:                                                        | N/A                                                                       |
| `currency`                                                                | [models.ExpenseLineItemCurrency](../models/expense-line-item-currency.md) | :heavy_minus_sign:                                                        | N/A                                                                       |
| `description`                                                             | *string*                                                                  | :heavy_minus_sign:                                                        | N/A                                                                       |
| `dimensions`                                                              | [models.DimensionInput](../models/dimension-input.md)[]                   | :heavy_minus_sign:                                                        | N/A                                                                       |
| `documentNumber`                                                          | *string*                                                                  | :heavy_minus_sign:                                                        | N/A                                                                       |
| `exchangeRate`                                                            | *number*                                                                  | :heavy_minus_sign:                                                        | N/A                                                                       |
| `itemId`                                                                  | *string*                                                                  | :heavy_minus_sign:                                                        | N/A                                                                       |
| `taxRate`                                                                 | [models.TaxRateInput](../models/tax-rate-input.md)                        | :heavy_minus_sign:                                                        | N/A                                                                       |
| `totalGrossAmount`                                                        | *number*                                                                  | :heavy_minus_sign:                                                        | N/A                                                                       |
| `totalNetAmount`                                                          | *number*                                                                  | :heavy_minus_sign:                                                        | N/A                                                                       |