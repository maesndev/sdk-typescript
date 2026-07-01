# JournalEntriesByBatchMetaDataResponseDto

## Example Usage

```typescript
import { JournalEntriesByBatchMetaDataResponseDto } from "@maesn/typescript-sdk/models";

let value: JournalEntriesByBatchMetaDataResponseDto = {
  id: "<id>",
  accountNumberLength: 5528.21,
  chartOfAccount: "<value>",
  createdDate: "<value>",
  entries: [
    {
      id: "<id>",
      accountId: "<id>",
      accountingPeriodId: "<id>",
      createdDate: "<value>",
      currency: "XDR",
      description: "inside rear dally and once tank farm qua",
      documentId: "<id>",
      files: [],
      isProvisional: true,
      journalCode: "<value>",
      journalLineItems: [
        {
          id: "<id>",
          accountCode: "<value>",
          accountId: "<id>",
          accountNumber: 6404.14,
          createdDate: null,
          currency: "CNY",
          customerId: null,
          debitCreditIndicator: "CREDIT",
          description: "till gee quaver deer",
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
          exchangeRate: 5036,
          supplierId: "<id>",
          taxRate: {
            id: "<id>",
            code: "<value>",
            name: "<value>",
            taxRatePercentage: "<value>",
          },
          thirdPartyCode: "<value>",
          totalGrossAmount: 2908.48,
          totalNetAmount: 2895.75,
          totalTaxAmount: 1900.76,
          updatedDate: null,
        },
      ],
      journalType: "<value>",
      number: "<value>",
      recordType: "STANDARD",
      transactionDate: "<value>",
      updatedDate: "<value>",
    },
  ],
  fiscalYearStartDate: "<value>",
  taskId: "<id>",
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `id`                                                                        | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `accountNumberLength`                                                       | *number*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `chartOfAccount`                                                            | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `createdDate`                                                               | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `entries`                                                                   | [models.JournalEntryResponseDto](../models/journal-entry-response-dto.md)[] | :heavy_check_mark:                                                          | N/A                                                                         |
| `fiscalYearStartDate`                                                       | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `taskId`                                                                    | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |