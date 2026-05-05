# BookingProposalResponseDto

## Example Usage

```typescript
import { BookingProposalResponseDto } from "@maesn/typescript-sdk/models";

let value: BookingProposalResponseDto = {
  id: "<id>",
  accountName: "<value>",
  addresses: [
    {},
  ],
  bankAccountId: "<id>",
  bankAccountNumber: 6703.15,
  bankCode: "<value>",
  bic: null,
  bookingProposalDate: "<value>",
  bookingType: null,
  contactAccountNumber: 4310.2,
  contactId: null,
  contactName: "<value>",
  createdDate: "<value>",
  currency: null,
  deliveryDate: "<value>",
  discountPaymentDate: null,
  discountPaymentDate2: "<value>",
  dueDate: "<value>",
  files: [],
  journalCode: "<value>",
  iban: "CH1330805D34098BT9209",
  isPaymentOrder: false,
  ledgerName: "<value>",
  lineItems: [
    {
      id: "<id>",
      accountCode: "<value>",
      accountId: null,
      accountName: "<value>",
      accountNumber: 6663.65,
      bookingTaxCode: null,
      createdDate: "<value>",
      description: "card pfft catalog along geez but uh-huh hence wherever",
      dimension1: "<value>",
      dimension2: "<value>",
      discountAmount: 9938.14,
      discountAmount2: 23.26,
      discountPercentage: 9085.21,
      discountPercentage2: 4905.52,
      taxCode: "<value>",
      taxRatePercentage: 6524.29,
      totalGrossAmount: 5480.15,
      totalNetAmount: 4492.57,
      updatedDate: "<value>",
    },
  ],
  notes: null,
  number: "<value>",
  orderId: "<id>",
  paidDate: "<value>",
  paymentTermsId: "<id>",
  status: "DISPUTED",
  taskId: "<id>",
  totalGrossAmount: 4868.44,
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