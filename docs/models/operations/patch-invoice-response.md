# PatchInvoiceResponse

Invoice updated successfully

## Example Usage

```typescript
import { PatchInvoiceResponse } from "@maesn/typescript-sdk/models/operations";

let value: PatchInvoiceResponse = {
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
  rawData: {},
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `meta`                                                                              | [operations.PatchInvoiceMeta](../../models/operations/patch-invoice-meta.md)        | :heavy_minus_sign:                                                                  | N/A                                                                                 |
| `data`                                                                              | [models.InvoiceResponseDto](../../models/invoice-response-dto.md)                   | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `errors`                                                                            | [operations.PatchInvoiceErrors](../../models/operations/patch-invoice-errors.md)    | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `rawData`                                                                           | [operations.PatchInvoiceRawData](../../models/operations/patch-invoice-raw-data.md) | :heavy_check_mark:                                                                  | N/A                                                                                 |