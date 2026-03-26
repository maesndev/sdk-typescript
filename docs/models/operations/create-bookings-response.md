# CreateBookingsResponse

## Example Usage

```typescript
import { CreateBookingsResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateBookingsResponse = {
  data: {
    id: null,
    accountNumberLength: 6333.51,
    chartOfAccount: "SKR14",
    createdDate: "<value>",
    entries: [],
    fiscalYearStartDate: "<value>",
    taskId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `meta`                                                                                  | [operations.CreateBookingsMeta](../../models/operations/create-bookings-meta.md)        | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `data`                                                                                  | [models.BookingsResponseDto](../../models/bookings-response-dto.md)                     | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `errors`                                                                                | [operations.CreateBookingsErrors](../../models/operations/create-bookings-errors.md)    | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `rawData`                                                                               | [operations.CreateBookingsRawData](../../models/operations/create-bookings-raw-data.md) | :heavy_check_mark:                                                                      | N/A                                                                                     |