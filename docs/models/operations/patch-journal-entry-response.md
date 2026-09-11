# PatchJournalEntryResponse

Journal entry updated successfully

## Example Usage

```typescript
import { PatchJournalEntryResponse } from "@maesn/typescript-sdk/models/operations";

let value: PatchJournalEntryResponse = {
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

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `meta`                                                                                         | [operations.PatchJournalEntryMeta](../../models/operations/patch-journal-entry-meta.md)        | :heavy_minus_sign:                                                                             | N/A                                                                                            |
| `data`                                                                                         | [models.JournalEntryResponseDto](../../models/journal-entry-response-dto.md)                   | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `errors`                                                                                       | [operations.PatchJournalEntryErrors](../../models/operations/patch-journal-entry-errors.md)    | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `rawData`                                                                                      | [operations.PatchJournalEntryRawData](../../models/operations/patch-journal-entry-raw-data.md) | :heavy_check_mark:                                                                             | N/A                                                                                            |