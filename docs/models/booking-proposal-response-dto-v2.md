# BookingProposalResponseDtoV2

## Example Usage

```typescript
import { BookingProposalResponseDtoV2 } from "@maesn/typescript-sdk/models";

let value: BookingProposalResponseDtoV2 = {
  id: "<id>",
  addresses: [
    {
      city: "Lake Magdalen",
    },
  ],
  bankAccount: {
    id: "<id>",
    bic: "<value>",
    code: "<value>",
    iban: null,
    number: 4935.74,
  },
  bookingProposalDate: "<value>",
  bookingType: "DOWN_PAYMENT",
  contact: {
    id: "<id>",
    accountNumber: 6023.09,
    name: "<value>",
  },
  createdDate: "<value>",
  currency: "Algerian Dinar",
  deliveryDate: "<value>",
  discountPaymentDate: "<value>",
  discountPaymentDate2: "<value>",
  dueDate: "<value>",
  files: [
    "<value 1>",
  ],
  journalCode: "<value>",
  isPaymentOrder: false,
  ledgerName: null,
  lineItems: [],
  notes: "<value>",
  number: "<value>",
  orderId: "<id>",
  paidDate: null,
  paymentTermId: "<id>",
  status: "PAID",
  totalGrossAmount: 9545.21,
  updatedDate: "<value>",
  vatId: "<id>",
};
```

## Fields

| Field                                                                                                        | Type                                                                                                         | Required                                                                                                     | Description                                                                                                  |
| ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                         | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `addresses`                                                                                                  | [models.BookingProposalAddressResponseDtoV2](../models/booking-proposal-address-response-dto-v2.md)[]        | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `bankAccount`                                                                                                | [models.BookingProposalResponseDtoV2BankAccount](../models/booking-proposal-response-dto-v2-bank-account.md) | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `bookingProposalDate`                                                                                        | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `bookingType`                                                                                                | [models.BookingProposalResponseDtoV2BookingType](../models/booking-proposal-response-dto-v2-booking-type.md) | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `contact`                                                                                                    | [models.Contact](../models/contact.md)                                                                       | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `createdDate`                                                                                                | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `currency`                                                                                                   | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `deliveryDate`                                                                                               | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `discountPaymentDate`                                                                                        | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `discountPaymentDate2`                                                                                       | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `dueDate`                                                                                                    | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `files`                                                                                                      | *string*[]                                                                                                   | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `journalCode`                                                                                                | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `isPaymentOrder`                                                                                             | *boolean*                                                                                                    | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `ledgerName`                                                                                                 | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `lineItems`                                                                                                  | [models.BookingProposalLineItemResponseDtoV2](../models/booking-proposal-line-item-response-dto-v2.md)[]     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `notes`                                                                                                      | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `number`                                                                                                     | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `orderId`                                                                                                    | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `paidDate`                                                                                                   | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `paymentTermId`                                                                                              | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `status`                                                                                                     | [models.BookingProposalResponseDtoV2Status](../models/booking-proposal-response-dto-v2-status.md)            | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `totalGrossAmount`                                                                                           | *number*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `updatedDate`                                                                                                | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `vatId`                                                                                                      | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |