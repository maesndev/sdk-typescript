# BookingEntryRequestDto

## Example Usage

```typescript
import { BookingEntryRequestDto } from "maesn/models";

let value: BookingEntryRequestDto = {
  accountNumber: 4450.75,
  amount: 6292.22,
  bookingDate: "<value>",
  bookingTaxCode: "<value>",
  bookingType: "ADVANCED_PAYMENT_RECEIVED",
  contraAccountNumber: 250.42,
  dimension1: "<value>",
  dimension2: "<value>",
  currency: "BRL",
  debitCreditIndicator: "DEBIT",
  description: "really lest inasmuch wing yowza yieldingly lustrous",
  documentNumber: "<value>",
  dueDate: "<value>",
  fileId: "<id>",
};
```

## Fields

| Field                                                                                                              | Type                                                                                                               | Required                                                                                                           | Description                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `accountNumber`                                                                                                    | *number*                                                                                                           | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `amount`                                                                                                           | *number*                                                                                                           | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `bookingDate`                                                                                                      | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `bookingTaxCode`                                                                                                   | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `bookingType`                                                                                                      | [models.BookingEntryRequestDtoBookingType](../models/booking-entry-request-dto-booking-type.md)                    | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `contraAccountNumber`                                                                                              | *number*                                                                                                           | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `dimension1`                                                                                                       | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `dimension2`                                                                                                       | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `currency`                                                                                                         | [models.BookingEntryRequestDtoCurrency](../models/booking-entry-request-dto-currency.md)                           | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `debitCreditIndicator`                                                                                             | [models.BookingEntryRequestDtoDebitCreditIndicator](../models/booking-entry-request-dto-debit-credit-indicator.md) | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `description`                                                                                                      | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `documentNumber`                                                                                                   | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `dueDate`                                                                                                          | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `fileId`                                                                                                           | *string*                                                                                                           | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |