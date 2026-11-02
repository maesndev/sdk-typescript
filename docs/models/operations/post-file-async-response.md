# PostFileAsyncResponse

File queued successfully. Processed asynchronously and returns 202 with taskId.

## Example Usage

```typescript
import { PostFileAsyncResponse } from "@maesn/typescript-sdk/models/operations";

let value: PostFileAsyncResponse = {
  data: {
    taskId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `meta`                                                                                 | [operations.PostFileAsyncMeta](../../models/operations/post-file-async-meta.md)        | :heavy_minus_sign:                                                                     | N/A                                                                                    |
| `data`                                                                                 | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                       | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `errors`                                                                               | [operations.PostFileAsyncErrors](../../models/operations/post-file-async-errors.md)    | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `rawData`                                                                              | [operations.PostFileAsyncRawData](../../models/operations/post-file-async-raw-data.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |