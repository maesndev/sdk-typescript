# CreateJournalEntryAttachmentsResponse

Journal entry attachment uploaded successfully

## Example Usage

```typescript
import { CreateJournalEntryAttachmentsResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateJournalEntryAttachmentsResponse = {
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
    files: [
      "<value 1>",
      "<value 2>",
    ],
    isProvisional: true,
    isReversal: false,
    journalCode: null,
    journalLineItems: [],
    journalType: "<value>",
    number: "<value>",
    recordType: "CLOSING",
    transactionDate: "<value>",
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                                   | Type                                                                                                                    | Required                                                                                                                | Description                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                                  | [operations.CreateJournalEntryAttachmentsMeta](../../models/operations/create-journal-entry-attachments-meta.md)        | :heavy_minus_sign:                                                                                                      | N/A                                                                                                                     |
| `data`                                                                                                                  | [models.JournalEntryResponseDto](../../models/journal-entry-response-dto.md)                                            | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     |
| `errors`                                                                                                                | [operations.CreateJournalEntryAttachmentsErrors](../../models/operations/create-journal-entry-attachments-errors.md)    | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     |
| `rawData`                                                                                                               | [operations.CreateJournalEntryAttachmentsRawData](../../models/operations/create-journal-entry-attachments-raw-data.md) | :heavy_check_mark:                                                                                                      | N/A                                                                                                                     |