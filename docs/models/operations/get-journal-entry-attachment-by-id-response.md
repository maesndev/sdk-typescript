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
    accountingReason: "IFRS",
    createdDate: "<value>",
    currency: "BRL",
    description:
      "gee unimpressively lest furthermore velocity egg likewise mid stint",
    documentId: "<id>",
    exchangeRate: "<value>",
    files: [
      "<value 1>",
    ],
    isProvisional: false,
    isReversal: true,
    journalCode: "<value>",
    journalLineItems: null,
    journalType: "<value>",
    number: "<value>",
    recordType: "CLOSING",
    transactionDate: "<value>",
    updatedDate: "<value>",
    version: "<value>",
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