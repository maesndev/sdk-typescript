# GetJournalEntryAttachmentByIdResponse

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
    journalLineItems: [],
    number: "<value>",
    transactionDate: "<value>",
    updatedDate: "<value>",
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