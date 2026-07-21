# JournalLineItem

## Example Usage

```typescript
import { JournalLineItem } from "@maesn/typescript-sdk/models";

let value: JournalLineItem = {
  id: null,
  accountCode: "<value>",
  accountId: "<id>",
  accountNumber: 7240.7,
  createdDate: "<value>",
  currency: "PLN",
  customerId: "<id>",
  debitCreditIndicator: "CREDIT",
  description: "onto ouch so",
  dimensions: [
    {
      id: "<id>",
      categoryName: "<value>",
      code: "<value>",
      name: "<value>",
    },
  ],
  documentId: "<id>",
  documentNumber: "<value>",
  exchangeRate: 3026.87,
  supplierId: "<id>",
  taxRate: null,
  thirdPartyCode: "<value>",
  totalGrossAmount: 6117.13,
  totalNetAmount: 4345.68,
  totalTaxAmount: 6967.36,
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                               | Type                                                                                                | Required                                                                                            | Description                                                                                         |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `id`                                                                                                | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `accountCode`                                                                                       | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `accountId`                                                                                         | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `accountNumber`                                                                                     | *number*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `createdDate`                                                                                       | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `currency`                                                                                          | [models.JournalLineItemCurrency](../models/journal-line-item-currency.md)                           | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `customerId`                                                                                        | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `debitCreditIndicator`                                                                              | [models.JournalLineItemDebitCreditIndicator](../models/journal-line-item-debit-credit-indicator.md) | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `description`                                                                                       | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `dimensions`                                                                                        | [models.Dimension](../models/dimension.md)[]                                                        | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `discountAmount`                                                                                    | *number*                                                                                            | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |
| `documentId`                                                                                        | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `documentNumber`                                                                                    | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `exchangeRate`                                                                                      | *number*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `supplierId`                                                                                        | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `taxRate`                                                                                           | [models.JournalLineItemTaxRate](../models/journal-line-item-tax-rate.md)                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `thirdPartyCode`                                                                                    | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `totalGrossAmount`                                                                                  | *number*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `totalNetAmount`                                                                                    | *number*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `totalTaxAmount`                                                                                    | *number*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `updatedDate`                                                                                       | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |