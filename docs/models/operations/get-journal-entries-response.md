# GetJournalEntriesResponse

## Example Usage

```typescript
import { GetJournalEntriesResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetJournalEntriesResponse = {
  data: [
    {
      id: "<id>",
      accountId: "<id>",
      accountingPeriodId: null,
      createdDate: "<value>",
      currency: "TND",
      description:
        "knottily stunning poorly rigid near duh for wriggler knight offensively",
      documentId: "<id>",
      files: [
        "<value 1>",
        "<value 2>",
      ],
      journalLineItems: [],
      number: "<value>",
      transactionDate: "<value>",
      updatedDate: "<value>",
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