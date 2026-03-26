# BookingEntryResponseDto

## Example Usage

```typescript
import { BookingEntryResponseDto } from "@maesn/typescript-sdk/models";

let value: BookingEntryResponseDto = {
  id: "<id>",
  accountNumber: 7445.77,
  amount: 3525.8,
  bookingDate: "<value>",
  bookingTaxCode: "<value>",
  bookingType: "PARTIAL_INVOICE",
  contraAccountNumber: 4500.77,
  dimension1: "<value>",
  dimension2: null,
  currency: "UZS",
  debitCreditIndicator: null,
  description: "beneath if past submitter in fooey if knottily tankful instead",
  documentNumber: "<value>",
  dueDate: "<value>",
  fileId: null,
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