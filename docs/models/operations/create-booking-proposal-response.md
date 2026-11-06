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
            amount: 4905.52,
          },
        ],
        discountAmount: 4836.78,
        discountAmount2: 9779.96,
        discountPercentage: 1507.56,
        discountPercentage2: 3147.39,
        taxCode: "<value>",
        taxRatePercentage: 5440.63,
        totalGrossAmount: 3316.85,
        totalNetAmount: 3153.6,
        type: "GOODS",
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
    totalGrossAmount: 1196.05,
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