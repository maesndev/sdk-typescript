# CreateSalesOrderAsyncResponse

Sales order creation queued successfully. Processed asynchronously and returns 202 with taskId.

## Example Usage

```typescript
import { CreateSalesOrderAsyncResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateSalesOrderAsyncResponse = {
  data: {
    taskId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                   | Type                                                                                                    | Required                                                                                                | Description                                                                                             |
| ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                  | [operations.CreateSalesOrderAsyncMeta](../../models/operations/create-sales-order-async-meta.md)        | :heavy_minus_sign:                                                                                      | N/A                                                                                                     |
| `data`                                                                                                  | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                                        | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `errors`                                                                                                | [operations.CreateSalesOrderAsyncErrors](../../models/operations/create-sales-order-async-errors.md)    | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `rawData`                                                                                               | [operations.CreateSalesOrderAsyncRawData](../../models/operations/create-sales-order-async-raw-data.md) | :heavy_check_mark:                                                                                      | N/A                                                                                                     |