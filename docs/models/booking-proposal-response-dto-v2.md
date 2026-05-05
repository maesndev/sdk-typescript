# BookingProposalResponseDtoV2

## Example Usage

```typescript
import { BookingProposalResponseDtoV2 } from "@maesn/typescript-sdk/models";

let value: BookingProposalResponseDtoV2 = {
  id: "<id>",
  addresses: [
    {
      city: null,
    },
  ],
  bankAccount: {
    id: "<id>",
    bic: "<value>",
    code: "<value>",
    iban: "MK37802448P89258A39",
    number: 8602.08,
  },
  bookingProposalDate: "<value>",
  bookingType: "EXPENSE",
  contact: {
    id: "<id>",
    accountNumber: 5605.39,
    name: "<value>",
  },
  createdDate: "<value>",
  currency: "Saint Helena Pound",
  deliveryDate: "<value>",
  discountPaymentDate: "<value>",
  discountPaymentDate2: "<value>",
  dueDate: "<value>",
  files: [
    "<value 1>",
    "<value 2>",
    "<value 3>",
  ],
  journalCode: "<value>",
  isPaymentOrder: true,
  ledgerName: "<value>",
  lineItems: [],
  notes: "<value>",
  number: null,
  orderId: "<id>",
  paidDate: "<value>",
  paymentTermId: "<id>",
  status: "VOIDED",
  totalGrossAmount: null,
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