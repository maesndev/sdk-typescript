# CreateJournalLineItem

## Example Usage

```typescript
import { CreateJournalLineItem } from "maesn/models";

let value: CreateJournalLineItem = {
  accountCode: "<value>",
  accountId: "<id>",
  accountNumber: 7827.36,
  currency: "CHF",
  customerId: "<id>",
  debitCreditIndicator: "CREDIT",
  description: "till woot function inasmuch as emotional mostly gleefully",
  dimensions: [
    "<value 1>",
  ],
  discountAmount: 7476.97,
  documentNumber: "<value>",
  exchangeRate: "<value>",
  supplierId: "<id>",
  taxRate: {
    id: "<id>",
    code: "<value>",
    name: "<value>",
    taxRatePercentage: "<value>",
  },
  thirdPartyCode: "<value>",
  totalGrossAmount: 6772.73,
  totalNetAmount: 3587.36,
  totalTaxAmount: 7575.73,
};
```

## Fields

| Field                                                                                                            | Type                                                                                                             | Required                                                                                                         | Description                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| `accountCode`                                                                                                    | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `accountId`                                                                                                      | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `accountNumber`                                                                                                  | *number*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `currency`                                                                                                       | [models.CreateJournalLineItemCurrency](../models/create-journal-line-item-currency.md)                           | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `customerId`                                                                                                     | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `debitCreditIndicator`                                                                                           | [models.CreateJournalLineItemDebitCreditIndicator](../models/create-journal-line-item-debit-credit-indicator.md) | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `description`                                                                                                    | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `dimensions`                                                                                                     | *string*[]                                                                                                       | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `discountAmount`                                                                                                 | *number*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `documentNumber`                                                                                                 | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `exchangeRate`                                                                                                   | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `supplierId`                                                                                                     | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `taxRate`                                                                                                        | [models.TaxRate](../models/tax-rate.md)                                                                          | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `thirdPartyCode`                                                                                                 | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `totalGrossAmount`                                                                                               | *number*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `totalNetAmount`                                                                                                 | *number*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `totalTaxAmount`                                                                                                 | *number*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |