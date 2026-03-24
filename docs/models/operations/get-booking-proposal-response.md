# GetBookingProposalResponse

## Example Usage

```typescript
import { GetBookingProposalResponse } from "maesn/models/operations";

let value: GetBookingProposalResponse = {
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
  data: [
    {
      id: "<id>",
      accountName: "<value>",
      addresses: [],
      bankAccountId: "<id>",
      bankAccountNumber: 5597.93,
      bankCode: "<value>",
      bic: "<value>",
      bookingProposalDate: "<value>",
      bookingType: "INVOICE",
      contactAccountNumber: 7020.44,
      contactId: "<id>",
      contactName: "<value>",
      createdDate: "<value>",
      currency: "Czech Koruna",
      deliveryDate: "<value>",
      discountPaymentDate: "<value>",
      discountPaymentDate2: "<value>",
      dueDate: "<value>",
      files: [
        "<value 1>",
      ],
      journalCode: "<value>",
      iban: "DK5220726123020435",
      isPaymentOrder: true,
      ledgerName: "<value>",
      lineItems: [],
      notes: "<value>",
      number: "<value>",
      orderId: "<id>",
      paidDate: "<value>",
      paymentTermsId: "<id>",
      status: "VOIDED",
      taskId: "<id>",
      totalGrossAmount: 695.99,
      updatedDate: "<value>",
      vatId: "<id>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `meta`                                                                                           | [models.MetaResponse](../../models/meta-response.md)                                             | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `data`                                                                                           | [models.BookingProposalResponseDto](../../models/booking-proposal-response-dto.md)[]             | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `errors`                                                                                         | [operations.GetBookingProposalErrors](../../models/operations/get-booking-proposal-errors.md)    | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `rawData`                                                                                        | [operations.GetBookingProposalRawData](../../models/operations/get-booking-proposal-raw-data.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |