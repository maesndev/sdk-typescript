# GetAsyncTaskInfoRequest

## Example Usage

```typescript
import { GetAsyncTaskInfoRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetAsyncTaskInfoRequest = {
  taskId: "<id>",
};
```

## Fields

| Field                                                         | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `taskId`                                                      | *string*                                                      | :heavy_check_mark:                                            | N/A                                                           |
| `companyId`                                                   | *string*                                                      | :heavy_minus_sign:                                            | ID of the company (required for multi-company target systems) |
| `page`                                                        | *number*                                                      | :heavy_minus_sign:                                            | N/A                                                           |
| `limit`                                                       | *number*                                                      | :heavy_minus_sign:                                            | N/A                                                           |