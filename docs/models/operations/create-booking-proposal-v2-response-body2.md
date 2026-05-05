# CreateBookingProposalV2ResponseBody2

Booking proposal queued successfully. Processed asynchronously and returns 202 with taskId.

## Example Usage

```typescript
import { CreateBookingProposalV2ResponseBody2 } from "@maesn/typescript-sdk/models/operations";

let value: CreateBookingProposalV2ResponseBody2 = {
  data: {
    taskId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                         | Type                                                                                                          | Required                                                                                                      | Description                                                                                                   |
| ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                        | [operations.CreateBookingProposalV2Meta2](../../models/operations/create-booking-proposal-v2-meta2.md)        | :heavy_minus_sign:                                                                                            | N/A                                                                                                           |
| `data`                                                                                                        | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                                              | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `errors`                                                                                                      | [operations.CreateBookingProposalV2Errors2](../../models/operations/create-booking-proposal-v2-errors2.md)    | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `rawData`                                                                                                     | [operations.CreateBookingProposalV2RawData2](../../models/operations/create-booking-proposal-v2-raw-data2.md) | :heavy_check_mark:                                                                                            | N/A                                                                                                           |