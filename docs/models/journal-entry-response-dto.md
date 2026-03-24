# JournalEntryResponseDto

## Example Usage

```typescript
import { JournalEntryResponseDto } from "maesn/models";

let value: JournalEntryResponseDto = {
  id: "<id>",
  accountId: "<id>",
  accountingPeriodId: "<id>",
  createdDate: "<value>",
  currency: "HTG",
  debitCreditIndicator: "DEBIT",
  deliveryDate: "<value>",
  description:
    "dismal positively quietly integer instead quietly apropos cleverly apropos",
  documentId: "<id>",
  dueDate: "<value>",
  exchangeRate: "<value>",
  files: [
    "<value 1>",
    "<value 2>",
    "<value 3>",
  ],
  isProvisional: true,
  journalCode: "<value>",
  journalLineItems: [],
  journalType: "<value>",
  number: "<value>",
  taxAssignmentDate: "<value>",
  transactionDate: "<value>",
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                                                | Type                                                                                                                 | Required                                                                                                             | Description                                                                                                          |
| -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                 | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `accountId`                                                                                                          | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `accountingPeriodId`                                                                                                 | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `createdDate`                                                                                                        | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `currency`                                                                                                           | [models.JournalEntryResponseDtoCurrency](../models/journal-entry-response-dto-currency.md)                           | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `debitCreditIndicator`                                                                                               | [models.JournalEntryResponseDtoDebitCreditIndicator](../models/journal-entry-response-dto-debit-credit-indicator.md) | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `deliveryDate`                                                                                                       | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `description`                                                                                                        | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `documentId`                                                                                                         | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `dueDate`                                                                                                            | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `exchangeRate`                                                                                                       | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `files`                                                                                                              | *string*[]                                                                                                           | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `isProvisional`                                                                                                      | *boolean*                                                                                                            | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `journalCode`                                                                                                        | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `journalLineItems`                                                                                                   | *string*[]                                                                                                           | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `journalType`                                                                                                        | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `number`                                                                                                             | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `taxAssignmentDate`                                                                                                  | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `transactionDate`                                                                                                    | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `updatedDate`                                                                                                        | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |