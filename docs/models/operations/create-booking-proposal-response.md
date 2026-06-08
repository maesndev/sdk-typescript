# CreateBookingProposalResponse

Booking proposal created successfully

## Example Usage

```typescript
import { CreateBookingProposalResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateBookingProposalResponse = {
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
        dimensions: [
          {
            id: "<id>",
            code: null,
            dimension: "<value>",
            name: "<value>",
          },
        ],
        discountAmount: 4905.52,
        discountAmount2: 4836.78,
        discountPercentage: 9779.96,
        discountPercentage2: 1507.56,
        taxCode: "<value>",
        taxRatePercentage: 1924.1,
        totalGrossAmount: 5440.63,
        totalNetAmount: 3316.85,
        type: "GOODS",
        updatedDate: "<value>",
      },
    ],
    notes: null,
    number: "<value>",
    orderId: "<id>",
    paidDate: "<value>",
    paymentTermsId: "<id>",
    status: "PARTIALLY_PAID",
    taskId: "<id>",
    totalGrossAmount: 4635.94,
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
| `meta`                                                                                                 | [operations.CreateBookingProposalMeta](../../models/operations/create-booking-proposal-meta.md)        | :heavy_minus_sign:                                                                                     | N/A                                                                                                    |
| `data`                                                                                                 | [models.BookingProposalResponseDto](../../models/booking-proposal-response-dto.md)                     | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `errors`                                                                                               | [operations.CreateBookingProposalErrors](../../models/operations/create-booking-proposal-errors.md)    | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `rawData`                                                                                              | [operations.CreateBookingProposalRawData](../../models/operations/create-booking-proposal-raw-data.md) | :heavy_check_mark:                                                                                     | N/A                                                                                                    |