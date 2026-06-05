# CreateJournalEntryResponse

Journal entry created successfully

## Example Usage

```typescript
import { CreateJournalEntryResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateJournalEntryResponse = {
  data: {
    id: "<id>",
    accountId: "<id>",
    accountingPeriodId: null,
    createdDate: "<value>",
    currency: "MKD",
    description: "barring around after meaningfully",
    documentId: null,
    files: [
      "<value 1>",
      "<value 2>",
      "<value 3>",
    ],
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
        documentNumber: "<value>",
        exchangeRate: 5782.76,
        supplierId: "<id>",
        taxRate: {
          id: "<id>",
          code: "<value>",
          name: "<value>",
          taxRatePercentage: "<value>",
        },
        thirdPartyCode: "<value>",
        totalGrossAmount: 6904.36,
        totalNetAmount: 1233.65,
        totalTaxAmount: 2727,
        updatedDate: "<value>",
      },
    ],
    journalType: "<value>",
    number: "<value>",
    transactionDate: "<value>",
    updatedDate: null,
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `meta`                                                                                           | [operations.CreateJournalEntryMeta](../../models/operations/create-journal-entry-meta.md)        | :heavy_minus_sign:                                                                               | N/A                                                                                              |
| `data`                                                                                           | [models.JournalEntryResponseDto](../../models/journal-entry-response-dto.md)                     | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `errors`                                                                                         | [operations.CreateJournalEntryErrors](../../models/operations/create-journal-entry-errors.md)    | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `rawData`                                                                                        | [operations.CreateJournalEntryRawData](../../models/operations/create-journal-entry-raw-data.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |