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
    fileId: "<id>",
    invoiceDate: "<value>",
    invoiceNumber: "<value>",
    invoiceType: "BILL",
    journalCode: "<value>",
    lineAmountTypes: "NOTAX",
    lineItems: [],
    name: "<value>",
    oneLineAddress: "<value>",
    openAmount: 4332.16,
    paidDate: null,
    paymentStatus: "UNKNOWN",
    paymentTermDuration: 3338.37,
    paymentTermId: "<id>",
    reference: "<value>",
    salesOrderId: "<id>",
    shippingDate: "<value>",
    status: "PARTIALLY_PAID",
    sumNetAmount: 5671.27,
    taxRule: "TAXFREE",
    totalAmount: 2368.02,
    totalTaxAmount: 8279.18,
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