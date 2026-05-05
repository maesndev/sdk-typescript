# CreateBookingProposalV2ResponseBody1

Booking proposal created successfully (synchronous).

## Example Usage

```typescript
import { CreateBookingProposalV2ResponseBody1 } from "@maesn/typescript-sdk/models/operations";

let value: CreateBookingProposalV2ResponseBody1 = {
  data: {
    id: null,
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
    currency: "Rufiyaa",
    deliveryDate: "<value>",
    discountPaymentDate: "<value>",
    discountPaymentDate2: "<value>",
    dueDate: "<value>",
    files: [
      "<value 1>",
      "<value 2>",
    ],
    journalCode: null,
    isPaymentOrder: true,
    ledgerName: "<value>",
    lineItems: [],
    notes: "<value>",
    number: "<value>",
    orderId: "<id>",
    paidDate: "<value>",
    paymentTermId: "<id>",
    status: "SUBMITTED",
    totalGrossAmount: 5062.84,
    updatedDate: "<value>",
    vatId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                         | Type                                                                                                          | Required                                                                                                      | Description                                                                                                   |
| ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                        | [operations.CreateBookingProposalV2Meta1](../../models/operations/create-booking-proposal-v2-meta1.md)        | :heavy_minus_sign:                                                                                            | N/A                                                                                                           |
| `data`                                                                                                        | [models.BookingProposalResponseDtoV2](../../models/booking-proposal-response-dto-v2.md)                       | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `errors`                                                                                                      | [operations.CreateBookingProposalV2Errors1](../../models/operations/create-booking-proposal-v2-errors1.md)    | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `rawData`                                                                                                     | [operations.CreateBookingProposalV2RawData1](../../models/operations/create-booking-proposal-v2-raw-data1.md) | :heavy_check_mark:                                                                                            | N/A                                                                                                           |