# BookingProposalResponseDtoV2

## Example Usage

```typescript
import { BookingProposalResponseDtoV2 } from "maesn/models";

let value: BookingProposalResponseDtoV2 = {
  id: "<id>",
  addresses: [],
  bankAccount: {
    id: "<id>",
    bic: "<value>",
    code: "<value>",
    iban: "FR280058058028153IU9D5G1Q49",
    number: 3558.3,
  },
  bookingProposalDate: "<value>",
  bookingType: "OTHER",
  contact: {
    id: "<id>",
    accountNumber: 549.02,
    name: "<value>",
  },
  createdDate: "<value>",
  currency: "Tugrik",
  deliveryDate: "<value>",
  discountPaymentDate: "<value>",
  discountPaymentDate2: "<value>",
  dueDate: "<value>",
  files: [
    "<value 1>",
    "<value 2>",
  ],
  journalCode: "<value>",
  isPaymentOrder: true,
  ledgerName: "<value>",
  lineItems: [
    {
      id: "<id>",
      account: {
        id: "<id>",
        code: "<value>",
        name: "<value>",
        number: 6594.9,
      },
      createdDate: "<value>",
      description: "developmental warp whenever whose footrest fooey oh",
      dimensions: [
        {
          id: "<id>",
          code: "<value>",
          dimension: "<value>",
          name: "<value>",
        },
      ],
      discountAmount: 4643.4,
      discountAmount2: 5667.37,
      discountPercentage: 7583.84,
      discountPercentage2: 1849.18,
      taxCode: "<value>",
      taxRatePercentage: 3247.36,
      totalGrossAmount: 7042.1,
      totalNetAmount: 3298.14,
      type: "SERVICE",
      updatedDate: "<value>",
    },
  ],
  notes: "<value>",
  number: "<value>",
  orderId: "<id>",
  paidDate: "<value>",
  paymentTermId: "<id>",
  status: "PARTIALLY_PAID",
  totalGrossAmount: 5443.53,
  updatedDate: "<value>",
  vatId: "<id>",
};
```

## Fields

| Field                                                                                                        | Type                                                                                                         | Required                                                                                                     | Description                                                                                                  |
| ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                         | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `addresses`                                                                                                  | [models.BookingProposalAddressResponseDtoV2](../models/booking-proposal-address-response-dto-v2.md)[]        | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `bankAccount`                                                                                                | [models.BankAccountResponseCommonDtoV2](../models/bank-account-response-common-dto-v2.md)                    | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `bookingProposalDate`                                                                                        | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `bookingType`                                                                                                | [models.BookingProposalResponseDtoV2BookingType](../models/booking-proposal-response-dto-v2-booking-type.md) | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `contact`                                                                                                    | [models.ContactResponseCommonDtoV2](../models/contact-response-common-dto-v2.md)                             | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
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