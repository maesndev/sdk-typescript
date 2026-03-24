# CreateBookingProposalV2Response

## Example Usage

```typescript
import { CreateBookingProposalV2Response } from "maesn/models/operations";

let value: CreateBookingProposalV2Response = {
  meta: {
    warnings: [
      "<value 1>",
      "<value 2>",
    ],
    pagination: {
      total: 3438.77,
      perPage: 5109.63,
      currentPage: 2626.79,
      totalPages: 3561.84,
    },
  },
  data: {
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
    bookingType: "CREDIT_NOTE",
    contact: {
      id: "<id>",
      accountNumber: 549.02,
      name: "<value>",
    },
    createdDate: "<value>",
    currency: "Libyan Dinar",
    deliveryDate: "<value>",
    discountPaymentDate: "<value>",
    discountPaymentDate2: "<value>",
    dueDate: "<value>",
    files: [
      "<value 1>",
    ],
    journalCode: "<value>",
    isPaymentOrder: false,
    ledgerName: "<value>",
    lineItems: [],
    notes: "<value>",
    number: "<value>",
    orderId: "<id>",
    paidDate: "<value>",
    paymentTermId: "<id>",
    status: "SUBMITTED",
    totalGrossAmount: 4494.92,
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
| `meta`                                                                                                      | [models.MetaResponse](../../models/meta-response.md)                                                        | :heavy_check_mark:                                                                                          | N/A                                                                                                         |
| `data`                                                                                                      | [models.BookingProposalResponseDtoV2](../../models/booking-proposal-response-dto-v2.md)                     | :heavy_check_mark:                                                                                          | N/A                                                                                                         |
| `errors`                                                                                                    | [operations.CreateBookingProposalV2Errors](../../models/operations/create-booking-proposal-v2-errors.md)    | :heavy_check_mark:                                                                                          | N/A                                                                                                         |
| `rawData`                                                                                                   | [operations.CreateBookingProposalV2RawData](../../models/operations/create-booking-proposal-v2-raw-data.md) | :heavy_check_mark:                                                                                          | N/A                                                                                                         |