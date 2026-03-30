# CreateJournalEntriesResponse

Journal entries created successfully in bulk

## Example Usage

```typescript
import { CreateJournalEntriesResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateJournalEntriesResponse = {
  data: {
    id: "<id>",
    accountNumberLength: 5500.73,
    chartOfAccount: "<value>",
    createdDate: "<value>",
    entries: [],
    fiscalYearStartDate: null,
    taskId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                              | Type                                                                                                               | Required                                                                                                           | Description                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `meta`                                                                                                             | [operations.CreateJournalEntriesMeta](../../models/operations/create-journal-entries-meta.md)                      | :heavy_minus_sign:                                                                                                 | N/A                                                                                                                |
| `data`                                                                                                             | [models.JournalEntriesByBatchMetaDataResponseDto](../../models/journal-entries-by-batch-meta-data-response-dto.md) | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `errors`                                                                                                           | [operations.CreateJournalEntriesErrors](../../models/operations/create-journal-entries-errors.md)                  | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `rawData`                                                                                                          | [operations.CreateJournalEntriesRawData](../../models/operations/create-journal-entries-raw-data.md)               | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |