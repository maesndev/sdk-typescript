# GetJournalEntryAttachmentsResponse

## Example Usage

```typescript
import { GetJournalEntryAttachmentsResponse } from "maesn/models/operations";

let value: GetJournalEntryAttachmentsResponse = {
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
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                             | Type                                                                                                              | Required                                                                                                          | Description                                                                                                       |
| ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                            | [models.MetaResponse](../../models/meta-response.md)                                                              | :heavy_check_mark:                                                                                                | N/A                                                                                                               |
| `data`                                                                                                            | [models.JournalEntryResponseDto](../../models/journal-entry-response-dto.md)[]                                    | :heavy_check_mark:                                                                                                | N/A                                                                                                               |
| `errors`                                                                                                          | [operations.GetJournalEntryAttachmentsErrors](../../models/operations/get-journal-entry-attachments-errors.md)    | :heavy_check_mark:                                                                                                | N/A                                                                                                               |
| `rawData`                                                                                                         | [operations.GetJournalEntryAttachmentsRawData](../../models/operations/get-journal-entry-attachments-raw-data.md) | :heavy_check_mark:                                                                                                | N/A                                                                                                               |