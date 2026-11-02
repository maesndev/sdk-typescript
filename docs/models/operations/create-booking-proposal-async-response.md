# CreateBookingProposalAsyncResponse

Booking proposal queued successfully. Processed asynchronously and returns 202 with taskId.

## Example Usage

```typescript
import { CreateBookingProposalAsyncResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateBookingProposalAsyncResponse = {
  data: {
    taskId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                             | Type                                                                                                              | Required                                                                                                          | Description                                                                                                       |
| ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                            | [operations.CreateBookingProposalAsyncMeta](../../models/operations/create-booking-proposal-async-meta.md)        | :heavy_minus_sign:                                                                                                | N/A                                                                                                               |
| `data`                                                                                                            | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                                                  | :heavy_check_mark:                                                                                                | N/A                                                                                                               |
| `errors`                                                                                                          | [operations.CreateBookingProposalAsyncErrors](../../models/operations/create-booking-proposal-async-errors.md)    | :heavy_check_mark:                                                                                                | N/A                                                                                                               |
| `rawData`                                                                                                         | [operations.CreateBookingProposalAsyncRawData](../../models/operations/create-booking-proposal-async-raw-data.md) | :heavy_check_mark:                                                                                                | N/A                                                                                                               |