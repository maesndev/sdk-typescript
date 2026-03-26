# GetBookingProposalResponse

## Example Usage

```typescript
import { GetBookingProposalResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetBookingProposalResponse = {
  data: {
    id: "<id>",
    accountName: "<value>",
    addresses: [],
    bankAccountId: "<id>",
    bankAccountNumber: 7234.15,
    bankCode: "<value>",
    bic: "<value>",
    bookingProposalDate: "<value>",
    bookingType: "INVOICE",
    contactAccountNumber: 6103.32,
    contactId: "<id>",
    contactName: "<value>",
    createdDate: "<value>",
    currency: "Forint",
    deliveryDate: "<value>",
    discountPaymentDate: "<value>",
    discountPaymentDate2: "<value>",
    dueDate: "<value>",
    files: null,
    journalCode: "<value>",
    iban: "BA885403852569640088",
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
    notes: "<value>",
    number: "<value>",
    orderId: "<id>",
    paidDate: "<value>",
    paymentTermsId: "<id>",
    status: "OPEN",
    taskId: "<id>",
    totalGrossAmount: null,
    updatedDate: "<value>",
    vatId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `meta`                                                                                           | [operations.GetBookingProposalMeta](../../models/operations/get-booking-proposal-meta.md)        | :heavy_minus_sign:                                                                               | N/A                                                                                              |
| `data`                                                                                           | [models.BookingProposalResponseDto](../../models/booking-proposal-response-dto.md)               | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `errors`                                                                                         | [operations.GetBookingProposalErrors](../../models/operations/get-booking-proposal-errors.md)    | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `rawData`                                                                                        | [operations.GetBookingProposalRawData](../../models/operations/get-booking-proposal-raw-data.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |