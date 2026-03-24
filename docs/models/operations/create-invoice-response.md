# CreateInvoiceResponse

## Example Usage

```typescript
import { CreateInvoiceResponse } from "maesn/models/operations";

let value: CreateInvoiceResponse = {
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
  data: {
    invoiceId: "<id>",
    addresses: [
      {
        addressLine1: "429 Walsh Tunnel",
        addressLine2: "-",
        city: "East Melyssa",
        countryCode: "AE",
        postalCode: "39193",
        type: "SELLING",
      },
    ],
    contactId: "<id>",
    createdDate: {},
    currency: "Czech Koruna",
    discountAmount: 8606.74,
    dueDate: {},
    fileId: "<id>",
    invoiceDate: {},
    invoiceNumber: "<value>",
    invoiceType: "BILL",
    journalCode: "<value>",
    lineAmountTypes: "NOTAX",
    lineItems: [],
    name: "<value>",
    oneLineAddress: "<value>",
    paidDate: {},
    paymentStatus: "PENDING",
    paymentTermDuration: 5586.05,
    paymentTermId: "<id>",
    reference: "<value>",
    shippingDate: {},
    status: "DOCUMENT_CREATED",
    sumNetAmount: 6822.71,
    taxRule: "OSS_GOODS",
    totalAmount: 5210.96,
    totalTaxAmount: 3349.61,
    updatedDate: {},
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [models.MetaResponse](../../models/meta-response.md)                                  | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `data`                                                                                | [models.InvoiceResponseDto](../../models/invoice-response-dto.md)                     | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.CreateInvoiceErrors](../../models/operations/create-invoice-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.CreateInvoiceRawData](../../models/operations/create-invoice-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |