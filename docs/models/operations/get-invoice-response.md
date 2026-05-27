# GetInvoiceResponse

Invoice record matching the provided ID

## Example Usage

```typescript
import { GetInvoiceResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetInvoiceResponse = {
  data: {
    id: "<id>",
    invoiceId: "<id>",
    addresses: [
      {},
    ],
    contactId: "<id>",
    createdDate: "<value>",
    currency: "Pataca",
    discountAmount: 6822.71,
    dueDate: "<value>",
    invoiceDate: "<value>",
    invoiceNumber: "<value>",
    invoiceType: "BILL",
    journalCode: "<value>",
    lineAmountTypes: "NOTAX",
    lineItems: [],
    name: "<value>",
    oneLineAddress: "<value>",
    paidDate: "<value>",
    paymentStatus: "DEBITED",
    paymentTermDuration: null,
    paymentTermId: "<id>",
    reference: "<value>",
    shippingDate: "<value>",
    status: "CORRECTIVE",
    sumNetAmount: 6171.07,
    taxRule: "OSS_SERVICES",
    totalAmount: 9258,
    totalTaxAmount: 7460.92,
    updatedDate: "<value>",
  },
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `meta`                                                                          | [operations.GetInvoiceMeta](../../models/operations/get-invoice-meta.md)        | :heavy_minus_sign:                                                              | N/A                                                                             |
| `data`                                                                          | [models.InvoiceResponseDto](../../models/invoice-response-dto.md)               | :heavy_check_mark:                                                              | N/A                                                                             |
| `errors`                                                                        | [operations.GetInvoiceErrors](../../models/operations/get-invoice-errors.md)    | :heavy_check_mark:                                                              | N/A                                                                             |
| `rawData`                                                                       | [operations.GetInvoiceRawData](../../models/operations/get-invoice-raw-data.md) | :heavy_check_mark:                                                              | N/A                                                                             |