# UpdateBookingProposalAsyncResponse

Booking proposal update request accepted for async processing

## Example Usage

```typescript
import { UpdateBookingProposalAsyncResponse } from "@maesn/typescript-sdk/models/operations";

let value: UpdateBookingProposalAsyncResponse = {
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
| `meta`                                                                                                            | [operations.UpdateBookingProposalAsyncMeta](../../models/operations/update-booking-proposal-async-meta.md)        | :heavy_minus_sign:                                                                                                | N/A                                                                                                               |
| `data`                                                                                                            | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                                                  | :heavy_check_mark:                                                                                                | N/A                                                                                                               |
| `errors`                                                                                                          | [operations.UpdateBookingProposalAsyncErrors](../../models/operations/update-booking-proposal-async-errors.md)    | :heavy_check_mark:                                                                                                | N/A                                                                                                               |
| `rawData`                                                                                                         | [operations.UpdateBookingProposalAsyncRawData](../../models/operations/update-booking-proposal-async-raw-data.md) | :heavy_check_mark:                                                                                                | N/A                                                                                                               |