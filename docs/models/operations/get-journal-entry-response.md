# GetJournalEntryResponse

Journal entry record matching the provided ID

## Example Usage

```typescript
import { GetJournalEntryResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetJournalEntryResponse = {
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

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `meta`                                                                                     | [operations.GetJournalEntryMeta](../../models/operations/get-journal-entry-meta.md)        | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.JournalEntryResponseDto](../../models/journal-entry-response-dto.md)               | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.GetJournalEntryErrors](../../models/operations/get-journal-entry-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.GetJournalEntryRawData](../../models/operations/get-journal-entry-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |