# GetBookingProposalsResponse

List of booking proposals for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetBookingProposalsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetBookingProposalsResponse = {
  data: [],
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                                              | Type                                                                                               | Required                                                                                           | Description                                                                                        |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| `meta`                                                                                             | [operations.GetBookingProposalsMeta](../../models/operations/get-booking-proposals-meta.md)        | :heavy_minus_sign:                                                                                 | N/A                                                                                                |
| `data`                                                                                             | [models.BookingProposalResponseDto](../../models/booking-proposal-response-dto.md)[]               | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `errors`                                                                                           | [operations.GetBookingProposalsErrors](../../models/operations/get-booking-proposals-errors.md)    | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `rawData`                                                                                          | [operations.GetBookingProposalsRawData](../../models/operations/get-booking-proposals-raw-data.md) | :heavy_check_mark:                                                                                 | N/A                                                                                                |