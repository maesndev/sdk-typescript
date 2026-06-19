# GetJournalEntriesAsyncResponse

Journal entries fetch queued successfully. Processed asynchronously and returns 202 with taskId.

## Example Usage

```typescript
import { GetJournalEntriesAsyncResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetJournalEntriesAsyncResponse = {
  data: {
    taskId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                     | Type                                                                                                      | Required                                                                                                  | Description                                                                                               |
| --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                    | [operations.GetJournalEntriesAsyncMeta](../../models/operations/get-journal-entries-async-meta.md)        | :heavy_minus_sign:                                                                                        | N/A                                                                                                       |
| `data`                                                                                                    | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                                          | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `errors`                                                                                                  | [operations.GetJournalEntriesAsyncErrors](../../models/operations/get-journal-entries-async-errors.md)    | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `rawData`                                                                                                 | [operations.GetJournalEntriesAsyncRawData](../../models/operations/get-journal-entries-async-raw-data.md) | :heavy_check_mark:                                                                                        | N/A                                                                                                       |