# GetAsyncTaskInfoResponse

## Example Usage

```typescript
import { GetAsyncTaskInfoResponse } from "maesn/models/operations";

let value: GetAsyncTaskInfoResponse = {
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
  data: {
    information: [
      {
        filename: "example.file",
        message: "<value>",
        timestamp: "<value>",
        type: "<value>",
      },
    ],
    responseData: {},
    status: "PARTIAL_SUCCESS",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `meta`                                                                                        | [models.MetaResponse](../../models/meta-response.md)                                          | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `data`                                                                                        | [models.AsyncTaskResponseDto](../../models/async-task-response-dto.md)                        | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `errors`                                                                                      | [operations.GetAsyncTaskInfoErrors](../../models/operations/get-async-task-info-errors.md)    | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `rawData`                                                                                     | [operations.GetAsyncTaskInfoRawData](../../models/operations/get-async-task-info-raw-data.md) | :heavy_check_mark:                                                                            | N/A                                                                                           |