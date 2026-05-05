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

### `operations.CreateBookingProposalV2ResponseBody2`

```typescript
const value: operations.CreateBookingProposalV2ResponseBody2 = {
  data: {
    taskId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

