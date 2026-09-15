# CreateBookingProposalV2Response


## Supported Types

### `operations.CreateBookingProposalV2ResponseBody1`

```typescript
const value: operations.CreateBookingProposalV2ResponseBody1 = {
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

### `operations.CreateBookingProposalV2ResponseBody2`

```typescript
const value: operations.CreateBookingProposalV2ResponseBody2 = {
  data: {
    taskId: "<id>",
    objectId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

