# JournalLineItem

## Example Usage

```typescript
import { JournalLineItem } from "@maesn/typescript-sdk/models";

let value: JournalLineItem = {
  id: null,
  accountCode: "<value>",
  accountId: "<id>",
  createdDate: "<value>",
  currency: "SCR",
  customerId: "<id>",
  debitCreditIndicator: "DEBIT",
  description: "bicycle ingratiate perfectly wealthy blossom possession mob",
  dimensions: [],
  documentNumber: "<value>",
  exchangeRate: 9089.64,
  supplierId: "<id>",
  taxRate: null,
  thirdPartyCode: "<value>",
  totalGrossAmount: 909.93,
  totalNetAmount: null,
  totalTaxAmount: 8325.18,
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                               | Type                                                                                                | Required                                                                                            | Description                                                                                         |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `id`                                                                                                | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `accountCode`                                                                                       | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `accountId`                                                                                         | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `accountNumber`                                                                                     | *number*                                                                                            | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |
| `createdDate`                                                                                       | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `currency`                                                                                          | [models.JournalLineItemCurrency](../models/journal-line-item-currency.md)                           | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `customerId`                                                                                        | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `debitCreditIndicator`                                                                              | [models.JournalLineItemDebitCreditIndicator](../models/journal-line-item-debit-credit-indicator.md) | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `description`                                                                                       | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `dimensions`                                                                                        | [models.Dimension](../models/dimension.md)[]                                                        | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `discountAmount`                                                                                    | *number*                                                                                            | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |
| `documentNumber`                                                                                    | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `exchangeRate`                                                                                      | *number*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `supplierId`                                                                                        | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `taxRate`                                                                                           | [models.JournalLineItemTaxRate](../models/journal-line-item-tax-rate.md)                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `thirdPartyCode`                                                                                    | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `totalGrossAmount`                                                                                  | *number*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `totalNetAmount`                                                                                    | *number*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `totalTaxAmount`                                                                                    | *number*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `updatedDate`                                                                                       | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |