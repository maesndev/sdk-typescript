# CreateBookingProposalV2Response

Booking proposal queued successfully. Processed asynchronously and returns 202 with taskId.

## Example Usage

```typescript
import { CreateBookingProposalV2Response } from "@maesn/typescript-sdk/models/operations";

let value: CreateBookingProposalV2Response = {
  data: {
    taskId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                       | Type                                                                                                        | Required                                                                                                    | Description                                                                                                 |
| ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                      | [operations.CreateBookingProposalV2Meta](../../models/operations/create-booking-proposal-v2-meta.md)        | :heavy_minus_sign:                                                                                          | N/A                                                                                                         |
| `data`                                                                                                      | [models.TaskIdResponseDto](../../models/task-id-response-dto.md)                                            | :heavy_check_mark:                                                                                          | N/A                                                                                                         |
| `errors`                                                                                                    | [operations.CreateBookingProposalV2Errors](../../models/operations/create-booking-proposal-v2-errors.md)    | :heavy_check_mark:                                                                                          | N/A                                                                                                         |
| `rawData`                                                                                                   | [operations.CreateBookingProposalV2RawData](../../models/operations/create-booking-proposal-v2-raw-data.md) | :heavy_check_mark:                                                                                          | N/A                                                                                                         |