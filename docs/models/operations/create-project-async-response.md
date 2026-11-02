# CreateProjectAsyncResponse

Project creation queued successfully. Processed asynchronously and returns 202 with taskId.

## Example Usage

```typescript
import { CreateProjectAsyncResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateProjectAsyncResponse = {
  data: {
    taskId: "<id>",
  },
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `meta`                                                                                           | [operations.CreateProjectAsyncMeta](../../models/operations/create-project-async-meta.md)        | :heavy_minus_sign:                                                                               | N/A                                                                                              |
| `data`                                                                                           | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                                 | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `errors`                                                                                         | [operations.CreateProjectAsyncErrors](../../models/operations/create-project-async-errors.md)    | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `rawData`                                                                                        | [operations.CreateProjectAsyncRawData](../../models/operations/create-project-async-raw-data.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |