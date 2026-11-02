# GetContactsAsyncResponse

Contacts fetch queued successfully. Processed asynchronously and returns 202 with taskId.

## Example Usage

```typescript
import { GetContactsAsyncResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetContactsAsyncResponse = {
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
| `meta`                                                                                       | [operations.GetContactsAsyncMeta](../../models/operations/get-contacts-async-meta.md)        | :heavy_minus_sign:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                             | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.GetContactsAsyncErrors](../../models/operations/get-contacts-async-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.GetContactsAsyncRawData](../../models/operations/get-contacts-async-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |