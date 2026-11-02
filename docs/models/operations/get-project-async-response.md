# GetProjectAsyncResponse

Project fetch queued successfully. Processed asynchronously and returns 202 with taskId.

## Example Usage

```typescript
import { GetProjectAsyncResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetProjectAsyncResponse = {
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
| `meta`                                                                                     | [operations.GetProjectAsyncMeta](../../models/operations/get-project-async-meta.md)        | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                           | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.GetProjectAsyncErrors](../../models/operations/get-project-async-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.GetProjectAsyncRawData](../../models/operations/get-project-async-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |