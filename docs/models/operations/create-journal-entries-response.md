# CreateJournalEntriesResponse

## Example Usage

```typescript
import { CreateJournalEntriesResponse } from "maesn/models/operations";

let value: CreateJournalEntriesResponse = {
  meta: {
    warnings: [
      "<value 1>",
      "<value 2>",
    ],
    pagination: {
      total: 3438.77,
      perPage: 5109.63,
      currentPage: 2626.79,
      totalPages: 3561.84,
    },
  },
  data: {
    id: "<id>",
    accountNumberLength: 3387.17,
    chartOfAccount: "<value>",
    createdDate: "<value>",
    entries: [],
    fiscalYearStartDate: "<value>",
    taskId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                              | Type                                                                                                               | Required                                                                                                           | Description                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `meta`                                                                                                             | [models.MetaResponse](../../models/meta-response.md)                                                               | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `data`                                                                                                             | [models.JournalEntriesByBatchMetaDataResponseDto](../../models/journal-entries-by-batch-meta-data-response-dto.md) | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `errors`                                                                                                           | [operations.CreateJournalEntriesErrors](../../models/operations/create-journal-entries-errors.md)                  | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `rawData`                                                                                                          | [operations.CreateJournalEntriesRawData](../../models/operations/create-journal-entries-raw-data.md)               | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |