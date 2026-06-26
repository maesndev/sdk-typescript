# GetProjectsAsyncResponse

Projects fetch queued successfully. Processed asynchronously and returns 202 with taskId.

## Example Usage

```typescript
import { GetProjectsAsyncResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetProjectsAsyncResponse = {
  data: {
    taskId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `meta`                                                                                       | [operations.GetProjectsAsyncMeta](../../models/operations/get-projects-async-meta.md)        | :heavy_minus_sign:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                             | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.GetProjectsAsyncErrors](../../models/operations/get-projects-async-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.GetProjectsAsyncRawData](../../models/operations/get-projects-async-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |