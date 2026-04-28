# CreateExpenseAsyncResponse

Expense queued successfully. Processed asynchronously and returns 202 with taskId.

## Example Usage

```typescript
import { CreateExpenseAsyncResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateExpenseAsyncResponse = {
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
| `meta`                                                                                           | [operations.CreateExpenseAsyncMeta](../../models/operations/create-expense-async-meta.md)        | :heavy_minus_sign:                                                                               | N/A                                                                                              |
| `data`                                                                                           | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                                 | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `errors`                                                                                         | [operations.CreateExpenseAsyncErrors](../../models/operations/create-expense-async-errors.md)    | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `rawData`                                                                                        | [operations.CreateExpenseAsyncRawData](../../models/operations/create-expense-async-raw-data.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |