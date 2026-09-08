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
      bankName: "<value>",
      bic: "<value>",
      code: "<value>",
      iban: "IS290004748580505080098962",
      number: 9730.03,
    },
    bookingProposalDate: "<value>",
    bookingType: "CREDIT_CARD",
    contact: {
      id: "<id>",
      accountNumber: 6103.19,
      name: "<value>",
    },
    createdDate: "<value>",
    currency: "Tugrik",
    deliveryDate: null,
    discountPaymentDate: "<value>",
    discountPaymentDate2: "<value>",
    dueDate: "<value>",
    files: [],
    generatorName: "<value>",
    journalCode: "<value>",
    isPaymentOrder: false,
    ledgerName: "<value>",
    lineItems: [],
    notes: "<value>",
    number: "<value>",
    orderId: "<id>",
    paidDate: "<value>",
    paymentTermId: "<id>",
    status: "VOIDED",
    totalGrossAmount: 947.09,
    updatedDate: "<value>",
    vatId: "<id>",
  },
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                                                         | Type                                                                                                          | Required                                                                                                      | Description                                                                                                   |
| ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                        | [operations.CreateBookingProposalV2Meta1](../../models/operations/create-booking-proposal-v2-meta1.md)        | :heavy_minus_sign:                                                                                            | N/A                                                                                                           |
| `data`                                                                                                        | [models.BookingProposalResponseDtoV2](../../models/booking-proposal-response-dto-v2.md)                       | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `errors`                                                                                                      | [operations.CreateBookingProposalV2Errors1](../../models/operations/create-booking-proposal-v2-errors1.md)    | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `rawData`                                                                                                     | [operations.CreateBookingProposalV2RawData1](../../models/operations/create-booking-proposal-v2-raw-data1.md) | :heavy_check_mark:                                                                                            | N/A                                                                                                           |