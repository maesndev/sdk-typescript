# CreateBookingProposalV2Response

Booking proposal created successfully. Returns 202 with taskId if processed asynchronously.

## Example Usage

```typescript
import { CreateBookingProposalV2Response } from "@maesn/typescript-sdk/models/operations";

let value: CreateBookingProposalV2Response = {
  data: {
    id: "<id>",
    addresses: [],
    bankAccount: {
      id: "<id>",
      bic: "<value>",
      code: "<value>",
      iban: null,
      number: 4935.74,
    },
    bookingProposalDate: "<value>",
    bookingType: "INVOICE",
    contact: {
      id: "<id>",
      accountNumber: 6023.09,
      name: "<value>",
    },
    createdDate: "<value>",
    currency: "Lek",
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
          number: 9138.81,
        },
        createdDate: "<value>",
        description: "across aside around",
        dimensions: [
          {
            id: "<id>",
            code: "<value>",
            dimension: "<value>",
            name: "<value>",
          },
        ],
        discountAmount: null,
        discountAmount2: 2887.21,
        discountPercentage: 575.94,
        discountPercentage2: null,
        taxCode: "<value>",
        taxRatePercentage: 1855.76,
        totalGrossAmount: 9506.34,
        totalNetAmount: 4674.01,
        type: null,
        updatedDate: "<value>",
      },
    ],
    notes: "<value>",
    number: "<value>",
    orderId: "<id>",
    paidDate: "<value>",
    paymentTermId: "<id>",
    status: "PARTIALLY_PAID",
    totalGrossAmount: 9946.8,
    updatedDate: "<value>",
    vatId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                       | Type                                                                                                        | Required                                                                                                    | Description                                                                                                 |
| ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                      | [operations.CreateBookingProposalV2Meta](../../models/operations/create-booking-proposal-v2-meta.md)        | :heavy_minus_sign:                                                                                          | N/A                                                                                                         |
| `data`                                                                                                      | [models.BookingProposalResponseDtoV2](../../models/booking-proposal-response-dto-v2.md)                     | :heavy_check_mark:                                                                                          | N/A                                                                                                         |
| `errors`                                                                                                    | [operations.CreateBookingProposalV2Errors](../../models/operations/create-booking-proposal-v2-errors.md)    | :heavy_check_mark:                                                                                          | N/A                                                                                                         |
| `rawData`                                                                                                   | [operations.CreateBookingProposalV2RawData](../../models/operations/create-booking-proposal-v2-raw-data.md) | :heavy_check_mark:                                                                                          | N/A                                                                                                         |