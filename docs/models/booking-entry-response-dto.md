# BookingEntryResponseDto

## Example Usage

```typescript
import { BookingEntryResponseDto } from "maesn/models";

let value: BookingEntryResponseDto = {
  id: "<id>",
  accountNumber: 2672.82,
  amount: 3273.87,
  bookingDate: "<value>",
  bookingTaxCode: "<value>",
  bookingType: "FINAL_INVOICE",
  contraAccountNumber: 3355.13,
  dimension1: "<value>",
  dimension2: "<value>",
  currency: "HKD",
  debitCreditIndicator: "DEBIT",
  description: "if minus climb woot",
  documentNumber: "<value>",
  dueDate: "<value>",
  fileId: "<id>",
};
```

## Fields

| Field                                                                                                                | Type                                                                                                                 | Required                                                                                                             | Description                                                                                                          |
| -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                                 | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `accountNumber`                                                                                                      | *number*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `amount`                                                                                                             | *number*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `bookingDate`                                                                                                        | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `bookingTaxCode`                                                                                                     | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `bookingType`                                                                                                        | [models.BookingEntryResponseDtoBookingType](../models/booking-entry-response-dto-booking-type.md)                    | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `contraAccountNumber`                                                                                                | *number*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `dimension1`                                                                                                         | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `dimension2`                                                                                                         | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `currency`                                                                                                           | [models.BookingEntryResponseDtoCurrency](../models/booking-entry-response-dto-currency.md)                           | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `debitCreditIndicator`                                                                                               | [models.BookingEntryResponseDtoDebitCreditIndicator](../models/booking-entry-response-dto-debit-credit-indicator.md) | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `description`                                                                                                        | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `documentNumber`                                                                                                     | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `dueDate`                                                                                                            | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |
| `fileId`                                                                                                             | *string*                                                                                                             | :heavy_check_mark:                                                                                                   | N/A                                                                                                                  |