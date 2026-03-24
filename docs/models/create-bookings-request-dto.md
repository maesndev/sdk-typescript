# CreateBookingsRequestDto

## Example Usage

```typescript
import { CreateBookingsRequestDto } from "maesn/models";

let value: CreateBookingsRequestDto = {
  accountNumberLength: 5460,
  chartOfAccount: "SKR42",
  entries: [
    {
      accountNumber: 2833.65,
      amount: 2531.3,
      bookingDate: "<value>",
      bookingTaxCode: "<value>",
      bookingType: "FINAL_INVOICE",
      contraAccountNumber: 6917.46,
      dimension1: "<value>",
      dimension2: "<value>",
      currency: "IDR",
      debitCreditIndicator: "CREDIT",
      description: "nor after once",
      documentNumber: "<value>",
      dueDate: "<value>",
      fileId: "<id>",
    },
  ],
  fiscalYearStartDate: "<value>",
};
```

## Fields

| Field                                                                                                      | Type                                                                                                       | Required                                                                                                   | Description                                                                                                |
| ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| `accountNumberLength`                                                                                      | *number*                                                                                                   | :heavy_check_mark:                                                                                         | N/A                                                                                                        |
| `chartOfAccount`                                                                                           | [models.CreateBookingsRequestDtoChartOfAccount](../models/create-bookings-request-dto-chart-of-account.md) | :heavy_check_mark:                                                                                         | N/A                                                                                                        |
| `entries`                                                                                                  | [models.BookingEntryRequestDto](../models/booking-entry-request-dto.md)[]                                  | :heavy_check_mark:                                                                                         | N/A                                                                                                        |
| `fiscalYearStartDate`                                                                                      | *string*                                                                                                   | :heavy_check_mark:                                                                                         | N/A                                                                                                        |