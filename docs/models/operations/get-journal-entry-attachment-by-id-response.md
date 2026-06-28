# GetJournalEntryAttachmentByIdResponse

Journal entry attachment record matching the provided ID

## Example Usage

```typescript
import { GetJournalEntryAttachmentByIdResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetJournalEntryAttachmentByIdResponse = {
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
    transactionDate: "<value>",
    updatedDate: null,
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                                     | Type                                                                                                                      | Required                                                                                                                  | Description                                                                                                               |
| ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                                    | [operations.GetJournalEntryAttachmentByIdMeta](../../models/operations/get-journal-entry-attachment-by-id-meta.md)        | :heavy_minus_sign:                                                                                                        | N/A                                                                                                                       |
| `data`                                                                                                                    | [models.JournalEntryResponseDto](../../models/journal-entry-response-dto.md)                                              | :heavy_check_mark:                                                                                                        | N/A                                                                                                                       |
| `errors`                                                                                                                  | [operations.GetJournalEntryAttachmentByIdErrors](../../models/operations/get-journal-entry-attachment-by-id-errors.md)    | :heavy_check_mark:                                                                                                        | N/A                                                                                                                       |
| `rawData`                                                                                                                 | [operations.GetJournalEntryAttachmentByIdRawData](../../models/operations/get-journal-entry-attachment-by-id-raw-data.md) | :heavy_check_mark:                                                                                                        | N/A                                                                                                                       |