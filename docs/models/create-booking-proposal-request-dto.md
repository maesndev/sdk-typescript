# CreateBookingProposalRequestDto

## Example Usage

```typescript
import { CreateBookingProposalRequestDto } from "maesn/models";

let value: CreateBookingProposalRequestDto = {
  id: "<id>",
  accountName: "<value>",
  addresses: [],
  bankAccountId: "<id>",
  bankAccountNumber: 2939.25,
  bankCode: "<value>",
  bic: "<value>",
  bookingProposalDate: "<value>",
  contactAccountNumber: 7736.46,
  contactId: "<id>",
  contactName: "<value>",
  currency: "Ouguiya",
  deliveryDate: "<value>",
  discountPaymentDate: "<value>",
  discountPaymentDate2: "<value>",
  dueDate: "<value>",
  journalCode: "<value>",
  iban: "TL523230520030850081946",
  isPaymentOrder: true,
  ledgerName: "<value>",
  lineItems: [],
  notes: "<value>",
  number: "<value>",
  orderId: "<id>",
  paidDate: "<value>",
  paymentTermsId: "<id>",
  status: "<value>",
  totalGrossAmount: 3625.61,
  vatId: "<id>",
};
```

## Fields

| Field                                                                    | Type                                                                     | Required                                                                 | Description                                                              |
| ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ |
| `id`                                                                     | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `accountName`                                                            | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `addresses`                                                              | [models.BookingProposalAddress](../models/booking-proposal-address.md)[] | :heavy_check_mark:                                                       | N/A                                                                      |
| `bankAccountId`                                                          | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `bankAccountNumber`                                                      | *number*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `bankCode`                                                               | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `bic`                                                                    | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `bookingProposalDate`                                                    | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `contactAccountNumber`                                                   | *number*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `contactId`                                                              | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `contactName`                                                            | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `currency`                                                               | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `deliveryDate`                                                           | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `discountPaymentDate`                                                    | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `discountPaymentDate2`                                                   | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `dueDate`                                                                | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `journalCode`                                                            | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `iban`                                                                   | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `isPaymentOrder`                                                         | *boolean*                                                                | :heavy_check_mark:                                                       | N/A                                                                      |
| `ledgerName`                                                             | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `lineItems`                                                              | [models.LineItemRequest](../models/line-item-request.md)[]               | :heavy_check_mark:                                                       | N/A                                                                      |
| `notes`                                                                  | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `number`                                                                 | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `orderId`                                                                | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `paidDate`                                                               | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `paymentTermsId`                                                         | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `status`                                                                 | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `totalGrossAmount`                                                       | *number*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `vatId`                                                                  | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |