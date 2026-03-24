# CreateBookingProposalResponse

## Example Usage

```typescript
import { CreateBookingProposalResponse } from "maesn/models/operations";

let value: CreateBookingProposalResponse = {
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
    accountName: "<value>",
    addresses: [],
    bankAccountId: "<id>",
    bankAccountNumber: 7286.06,
    bankCode: "<value>",
    bic: "<value>",
    bookingProposalDate: "<value>",
    bookingType: "OTHER",
    contactAccountNumber: 1341.06,
    contactId: "<id>",
    contactName: "<value>",
    createdDate: "<value>",
    currency: "Singapore Dollar",
    deliveryDate: "<value>",
    discountPaymentDate: "<value>",
    discountPaymentDate2: "<value>",
    dueDate: "<value>",
    files: [],
    journalCode: "<value>",
    iban: "PK04JEQX0695530500540385",
    isPaymentOrder: false,
    ledgerName: "<value>",
    lineItems: [],
    notes: "<value>",
    number: "<value>",
    orderId: "<id>",
    paidDate: "<value>",
    paymentTermsId: "<id>",
    status: "CANCELLED",
    taskId: "<id>",
    totalGrossAmount: 5346.08,
    updatedDate: "<value>",
    vatId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                  | Type                                                                                                   | Required                                                                                               | Description                                                                                            |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ |
| `meta`                                                                                                 | [models.MetaResponse](../../models/meta-response.md)                                                   | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `data`                                                                                                 | [models.BookingProposalResponseDto](../../models/booking-proposal-response-dto.md)                     | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `errors`                                                                                               | [operations.CreateBookingProposalErrors](../../models/operations/create-booking-proposal-errors.md)    | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `rawData`                                                                                              | [operations.CreateBookingProposalRawData](../../models/operations/create-booking-proposal-raw-data.md) | :heavy_check_mark:                                                                                     | N/A                                                                                                    |