# GetJournalEntryResponse

## Example Usage

```typescript
import { GetJournalEntryResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetJournalEntryResponse = {
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

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `meta`                                                                                     | [operations.GetJournalEntryMeta](../../models/operations/get-journal-entry-meta.md)        | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.JournalEntryResponseDto](../../models/journal-entry-response-dto.md)               | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.GetJournalEntryErrors](../../models/operations/get-journal-entry-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.GetJournalEntryRawData](../../models/operations/get-journal-entry-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |