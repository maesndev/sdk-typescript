# GetJournalEntriesResponse

List of journal entries for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetJournalEntriesResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetJournalEntriesResponse = {
  data: [
    {
      id: "<id>",
      accountId: "<id>",
      accountingPeriodId: null,
      accountingReason: "CALCULATION",
      createdDate: "<value>",
      currency: "VEB",
      description:
        "mutate austere under close helpless enthusiastically humor total",
      documentId: null,
      exchangeRate: "<value>",
      files: [
        "<value 1>",
        "<value 2>",
      ],
      isProvisional: true,
      isReversal: false,
      journalCode: "<value>",
      journalLineItems: [],
      journalType: "<value>",
      number: "<value>",
      recordType: "CLOSING",
      transactionDate: "<value>",
      updatedDate: "<value>",
      version: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `meta`                                                                                         | [operations.GetJournalEntriesMeta](../../models/operations/get-journal-entries-meta.md)        | :heavy_minus_sign:                                                                             | N/A                                                                                            |
| `data`                                                                                         | [models.JournalEntryResponseDto](../../models/journal-entry-response-dto.md)[]                 | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `errors`                                                                                       | [operations.GetJournalEntriesErrors](../../models/operations/get-journal-entries-errors.md)    | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `rawData`                                                                                      | [operations.GetJournalEntriesRawData](../../models/operations/get-journal-entries-raw-data.md) | :heavy_check_mark:                                                                             | N/A                                                                                            |