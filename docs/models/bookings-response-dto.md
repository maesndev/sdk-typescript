# BookingsResponseDto

## Example Usage

```typescript
import { BookingsResponseDto } from "@maesn/typescript-sdk/models";

let value: BookingsResponseDto = {
  id: "<id>",
  accountNumberLength: 2652.68,
  chartOfAccount: "SKR04",
  createdDate: "<value>",
  entries: [
    {
      id: "<id>",
      accountNumber: 7906.27,
      amount: 2304.7,
      bookingDate: "<value>",
      bookingTaxCode: null,
      bookingType: "ADVANCED_PAYMENT_RECEIVED",
      contraAccountNumber: 8538.46,
      dimension1: "<value>",
      dimension2: "<value>",
      currency: null,
      debitCreditIndicator: null,
      description: "out provided jubilantly phooey whether thread boo",
      documentNumber: "<value>",
      dueDate: "<value>",
      fileId: "<id>",
    },
  ],
  fiscalYearStartDate: "<value>",
  taskId: "<id>",
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `id`                                                                                            | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `accountNumberLength`                                                                           | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `chartOfAccount`                                                                                | [models.BookingsResponseDtoChartOfAccount](../models/bookings-response-dto-chart-of-account.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `createdDate`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `entries`                                                                                       | [models.BookingEntryResponseDto](../models/booking-entry-response-dto.md)[]                     | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `fiscalYearStartDate`                                                                           | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `taskId`                                                                                        | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |