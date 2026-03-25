# CreateInvoiceRequest

## Example Usage

```typescript
import { CreateInvoiceRequest } from "maesn/models/operations";

let value: CreateInvoiceRequest = {
  body: {
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
    currency: "Dalasi",
    discountPercentage: 4037.08,
    dueDate: "<value>",
    fileId: "<id>",
    grossTotalAmount: 2605.57,
    invoiceDate: "<value>",
    invoiceNumber: "<value>",
    invoiceType: "STANDARD",
    journalCode: "<value>",
    lineAmountTypes: "<value>",
    lineItems: [
      {
        accountCode: "<value>",
        accountId: "<id>",
        description:
          "punctually habit until handsome till via nougat inside than",
        dimensions: [
          {
            id: "<id>",
            categoryName: "<value>",
            name: "<value>",
          },
        ],
        discountItemPercentage: 561.24,
        grossAmount: 9717.96,
        itemId: "<id>",
        name: "<value>",
        quantity: 4470.61,
        taxCode: "<value>",
        taxRatePercentage: 8595.29,
        taxType: "<value>",
        type: "<value>",
        unitAmount: 532.74,
        unitName: "<value>",
      },
    ],
    name: "<value>",
    oneLineAddress: "<value>",
    paidDate: "<value>",
    paymentTermDuration: 5581.49,
    paymentTermId: "<id>",
    reference: "<value>",
    shippingDate: "<value>",
    shippingType: "SERVICEPERIOD",
    shippingEndDate: "<value>",
    status: "OVERDUE",
    taxRule: "OSS_GOODS",
    taxText: "<value>",
  },
};
```

## Fields

| Field                                                                        | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `environmentName`                                                            | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `companyId`                                                                  | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `body`                                                                       | [models.CreateInvoiceRequestDto](../../models/create-invoice-request-dto.md) | :heavy_check_mark:                                                           | N/A                                                                          |