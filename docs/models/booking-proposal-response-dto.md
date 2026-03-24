# BookingProposalResponseDto

## Example Usage

```typescript
import { BookingProposalResponseDto } from "maesn/models";

let value: BookingProposalResponseDto = {
  id: "<id>",
  accountName: "<value>",
  addresses: [
    {},
  ],
  bankAccountId: "<id>",
  bankAccountNumber: 8275.78,
  bankCode: "<value>",
  bic: "<value>",
  bookingProposalDate: "<value>",
  bookingType: "BILL",
  contactAccountNumber: 9058.69,
  contactId: "<id>",
  contactName: "<value>",
  createdDate: "<value>",
  currency: "Metical",
  deliveryDate: "<value>",
  discountPaymentDate: "<value>",
  discountPaymentDate2: "<value>",
  dueDate: "<value>",
  files: [
    "<value 1>",
    "<value 2>",
  ],
  journalCode: "<value>",
  iban: "MD4100L8A0509V1U5D34098B",
  isPaymentOrder: false,
  ledgerName: "<value>",
  lineItems: [
    {
      id: "<id>",
      accountCode: "<value>",
      accountId: "<id>",
      accountName: "<value>",
      accountNumber: 6316.58,
      bookingTaxCode: "<value>",
      createdDate: "<value>",
      description:
        "king gosh low encode vast palate viability decisive uh-huh worth",
      dimension1: "<value>",
      dimension2: "<value>",
      discountAmount: 4425.76,
      discountAmount2: 3540.21,
      discountPercentage: 1931.44,
      discountPercentage2: 666.84,
      taxCode: "<value>",
      taxRatePercentage: 1189.37,
      totalGrossAmount: 9169.21,
      totalNetAmount: 4106.28,
      type: "SERVICES",
      updatedDate: "<value>",
    },
  ],
  notes: "<value>",
  number: "<value>",
  orderId: "<id>",
  paidDate: "<value>",
  paymentTermsId: "<id>",
  status: "SUBMITTED",
  taskId: "<id>",
  totalGrossAmount: 8492.93,
  updatedDate: "<value>",
  vatId: "<id>",
};
```

## Fields

| Field                                                                                                   | Type                                                                                                    | Required                                                                                                | Description                                                                                             |
| ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                    | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `accountName`                                                                                           | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `addresses`                                                                                             | [models.BookingProposalAddress](../models/booking-proposal-address.md)[]                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `bankAccountId`                                                                                         | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `bankAccountNumber`                                                                                     | *number*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `bankCode`                                                                                              | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `bic`                                                                                                   | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `bookingProposalDate`                                                                                   | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `bookingType`                                                                                           | [models.BookingProposalResponseDtoBookingType](../models/booking-proposal-response-dto-booking-type.md) | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `contactAccountNumber`                                                                                  | *number*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `contactId`                                                                                             | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `contactName`                                                                                           | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `createdDate`                                                                                           | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `currency`                                                                                              | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `deliveryDate`                                                                                          | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `discountPaymentDate`                                                                                   | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `discountPaymentDate2`                                                                                  | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `dueDate`                                                                                               | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `files`                                                                                                 | *string*[]                                                                                              | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `journalCode`                                                                                           | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `iban`                                                                                                  | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `isPaymentOrder`                                                                                        | *boolean*                                                                                               | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `ledgerName`                                                                                            | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `lineItems`                                                                                             | [models.LineItemResponse](../models/line-item-response.md)[]                                            | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `notes`                                                                                                 | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `number`                                                                                                | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `orderId`                                                                                               | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `paidDate`                                                                                              | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `paymentTermsId`                                                                                        | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `status`                                                                                                | [models.BookingProposalResponseDtoStatus](../models/booking-proposal-response-dto-status.md)            | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `taskId`                                                                                                | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `totalGrossAmount`                                                                                      | *number*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `updatedDate`                                                                                           | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |
| `vatId`                                                                                                 | *string*                                                                                                | :heavy_check_mark:                                                                                      | N/A                                                                                                     |