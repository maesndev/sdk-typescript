# GetAsyncTaskInfoResponse

Async task status and result matching the provided task ID

## Example Usage

```typescript
import { GetAsyncTaskInfoResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetAsyncTaskInfoResponse = {
  data: {
    information: [
      {
        filename: "example.file",
        message: "<value>",
        timestamp: "<value>",
        type: null,
      },
    ],
    responseData: {},
    status: "SUCCESS",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `meta`                                                                                        | [operations.GetAsyncTaskInfoMeta](../../models/operations/get-async-task-info-meta.md)        | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `data`                                                                                        | [models.AsyncTaskResponseDto](../../models/async-task-response-dto.md)                        | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `errors`                                                                                      | [operations.GetAsyncTaskInfoErrors](../../models/operations/get-async-task-info-errors.md)    | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `rawData`                                                                                     | [operations.GetAsyncTaskInfoRawData](../../models/operations/get-async-task-info-raw-data.md) | :heavy_check_mark:                                                                            | N/A                                                                                           |