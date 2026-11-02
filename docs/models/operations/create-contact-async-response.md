# CreateContactAsyncResponse

Contact creation queued successfully. Processed asynchronously and returns 202 with taskId.

## Example Usage

```typescript
import { CreateContactAsyncResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateContactAsyncResponse = {
  data: {
    taskId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `meta`                                                                                           | [operations.CreateContactAsyncMeta](../../models/operations/create-contact-async-meta.md)        | :heavy_minus_sign:                                                                               | N/A                                                                                              |
| `data`                                                                                           | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                                 | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `errors`                                                                                         | [operations.CreateContactAsyncErrors](../../models/operations/create-contact-async-errors.md)    | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `rawData`                                                                                        | [operations.CreateContactAsyncRawData](../../models/operations/create-contact-async-raw-data.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |