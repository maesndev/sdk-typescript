# CreateBookingProposalRequestDtoV2

## Example Usage

```typescript
import { CreateBookingProposalRequestDtoV2 } from "maesn/models";

let value: CreateBookingProposalRequestDtoV2 = {
  id: "<id>",
  addresses: [],
  bankAccount: {
    id: "<id>",
    bic: "<value>",
    code: "<value>",
    iban: "BH67ERNK82599HX30D6234",
    number: 7514.89,
  },
  bookingProposalDate: "<value>",
  contact: {
    id: "<id>",
    accountNumber: 4325.54,
    name: "<value>",
  },
  currency: "Iranian Rial",
  deliveryDate: "<value>",
  discountPaymentDate: "<value>",
  discountPaymentDate2: "<value>",
  dueDate: "<value>",
  journalCode: "<value>",
  isPaymentOrder: true,
  ledgerName: "<value>",
  lineItems: [],
  notes: "<value>",
  number: "<value>",
  orderId: "<id>",
  paidDate: "<value>",
  paymentTermId: "<id>",
  status: "OPEN",
  totalGrossAmount: 8571.14,
  vatId: "<id>",
};
```

## Fields

| Field                                                                                                        | Type                                                                                                         | Required                                                                                                     | Description                                                                                                  |
| ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                         | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `addresses`                                                                                                  | [models.BookingProposalAddressRequestDtoV2](../models/booking-proposal-address-request-dto-v2.md)[]          | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `bankAccount`                                                                                                | [models.BankAccountRequestCommonDtoV2](../models/bank-account-request-common-dto-v2.md)                      | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `bookingProposalDate`                                                                                        | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `contact`                                                                                                    | [models.ContactRequestCommonDtoV2](../models/contact-request-common-dto-v2.md)                               | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `currency`                                                                                                   | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `deliveryDate`                                                                                               | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `discountPaymentDate`                                                                                        | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `discountPaymentDate2`                                                                                       | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `dueDate`                                                                                                    | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `journalCode`                                                                                                | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `isPaymentOrder`                                                                                             | *boolean*                                                                                                    | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `ledgerName`                                                                                                 | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `lineItems`                                                                                                  | [models.BookingProposalLineItemRequestDtoV2](../models/booking-proposal-line-item-request-dto-v2.md)[]       | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `notes`                                                                                                      | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `number`                                                                                                     | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `orderId`                                                                                                    | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `paidDate`                                                                                                   | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `paymentTermId`                                                                                              | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `status`                                                                                                     | [models.CreateBookingProposalRequestDtoV2Status](../models/create-booking-proposal-request-dto-v2-status.md) | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `totalGrossAmount`                                                                                           | *number*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `vatId`                                                                                                      | *string*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |