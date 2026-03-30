# CreateInvoiceResponse

Invoice created successfully

## Example Usage

```typescript
import { CreateInvoiceResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateInvoiceResponse = {
  data: {
    invoiceId: "<id>",
    addresses: [
      {},
    ],
    contactId: "<id>",
    createdDate: "<value>",
    currency: "Congolese Franc",
    discountAmount: 3702.79,
    dueDate: "<value>",
    invoiceDate: "<value>",
    invoiceNumber: "<value>",
    invoiceType: "STANDARD",
    journalCode: "<value>",
    lineAmountTypes: "EXCLUSIVE",
    lineItems: [
      {
        lineItemId: "<id>",
        accountId: "<id>",
        createdDate: "<value>",
        description: "diligently odd ah zowie even avow wilt stealthily",
        dimensions: [
          {
            id: "<id>",
            categoryName: "<value>",
            name: null,
          },
        ],
        discountItemAmount: 2836.31,
        discountItemPercentage: 6807.55,
        grossAmount: 805.04,
        itemsAmount: 4417.2,
        itemId: "<id>",
        name: "<value>",
        quantity: 985.86,
        taxRatePercentage: 688.21,
        unitAmount: 2381.59,
        updatedDate: "<value>",
      },
    ],
    name: "<value>",
    oneLineAddress: "<value>",
    paidDate: "<value>",
    paymentStatus: "PENDING",
    paymentTermDuration: 6692.63,
    paymentTermId: "<id>",
    reference: null,
    shippingDate: "<value>",
    status: "OVERDUE",
    sumNetAmount: 7325.9,
    taxRule: null,
    totalAmount: 9987.02,
    totalTaxAmount: 1923.54,
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [operations.CreateInvoiceMeta](../../models/operations/create-invoice-meta.md)        | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `data`                                                                                | [models.InvoiceResponseDto](../../models/invoice-response-dto.md)                     | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.CreateInvoiceErrors](../../models/operations/create-invoice-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.CreateInvoiceRawData](../../models/operations/create-invoice-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |