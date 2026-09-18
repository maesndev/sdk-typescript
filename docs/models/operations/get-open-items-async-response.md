# GetOpenItemsAsyncResponse

Open items fetch queued successfully. Processed asynchronously and returns 202 with taskId.

## Example Usage

```typescript
import { GetOpenItemsAsyncResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetOpenItemsAsyncResponse = {
  data: {
    taskId: "<id>",
    objectId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `meta`                                                                                          | [operations.GetOpenItemsAsyncMeta](../../models/operations/get-open-items-async-meta.md)        | :heavy_minus_sign:                                                                              | N/A                                                                                             |
| `data`                                                                                          | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                                | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `errors`                                                                                        | [operations.GetOpenItemsAsyncErrors](../../models/operations/get-open-items-async-errors.md)    | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `rawData`                                                                                       | [operations.GetOpenItemsAsyncRawData](../../models/operations/get-open-items-async-raw-data.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |