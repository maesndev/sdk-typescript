# GetContactAsyncResponse

Contact fetch queued successfully. Processed asynchronously and returns 202 with taskId.

## Example Usage

```typescript
import { GetContactAsyncResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetContactAsyncResponse = {
  data: {
    taskId: "<id>",
  },
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `meta`                                                                                     | [operations.GetContactAsyncMeta](../../models/operations/get-contact-async-meta.md)        | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                           | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.GetContactAsyncErrors](../../models/operations/get-contact-async-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.GetContactAsyncRawData](../../models/operations/get-contact-async-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |