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
    paidDate: "<value>",
    paymentStatus: "NO_OPEN_ITEM",
    paymentTermDuration: 9246.75,
    paymentTermId: "<id>",
    reference: "<value>",
    shippingDate: "<value>",
    status: "PAID",
    sumNetAmount: 9803.41,
    taxRule: "OSS_ELECTRONIC_SERVICES",
    totalAmount: 7460.92,
    totalTaxAmount: 4094.65,
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