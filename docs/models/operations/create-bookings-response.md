# CreateBookingsResponse

## Example Usage

```typescript
import { CreateBookingsResponse } from "maesn/models/operations";

let value: CreateBookingsResponse = {
  meta: {
    warnings: [
      "<value 1>",
      "<value 2>",
    ],
    pagination: {
      total: 3438.77,
      perPage: 5109.63,
      currentPage: 2626.79,
      totalPages: 3561.84,
    },
  },
  data: {
    id: "<id>",
    accountNumberLength: 205.38,
    chartOfAccount: "SKR42",
    createdDate: "<value>",
    entries: [
      {
        id: "<id>",
        accountNumber: 8014.8,
        amount: 8390.99,
        bookingDate: "<value>",
        bookingTaxCode: "<value>",
        bookingType: "PARTIAL_INVOICE",
        contraAccountNumber: 7764.27,
        dimension1: "<value>",
        dimension2: "<value>",
        currency: "DKK",
        debitCreditIndicator: "DEBIT",
        description:
          "astride large productive lobster middle whereas westernise positively irk",
        documentNumber: "<value>",
        dueDate: "<value>",
        fileId: "<id>",
      },
    ],
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
| `meta`                                                                                  | [models.MetaResponse](../../models/meta-response.md)                                    | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `data`                                                                                  | [models.BookingsResponseDto](../../models/bookings-response-dto.md)                     | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `errors`                                                                                | [operations.CreateBookingsErrors](../../models/operations/create-bookings-errors.md)    | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `rawData`                                                                               | [operations.CreateBookingsRawData](../../models/operations/create-bookings-raw-data.md) | :heavy_check_mark:                                                                      | N/A                                                                                     |