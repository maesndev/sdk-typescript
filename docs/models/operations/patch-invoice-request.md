# PatchInvoiceRequest

## Example Usage

```typescript
import { PatchInvoiceRequest } from "maesn/models/operations";

let value: PatchInvoiceRequest = {
  invoiceId: "<id>",
  body: {
    invoiceId: "<id>",
    contactId: "<id>",
    name: "<value>",
    reference: "<value>",
    currency: "Cedi",
    invoiceDate: "<value>",
    journalCode: "<value>",
    paymentTermId: "<id>",
    fileId: "<id>",
    status: "VOIDED",
    invoiceType: "BILL",
    oneLineAddress: "<value>",
    addresses: [],
    taxRule: "NOTEU",
    taxText: "<value>",
    lineItems: [
      {
        lineItemId: "<id>",
        itemId: "<id>",
        unitName: "<value>",
        type: "TEXT",
        quantity: 9977.96,
        taxRatePercentage: 1732.6,
        unitAmount: 4843.17,
        grossAmount: 5724,
        taxCode: "<value>",
        taxType: "<value>",
        description:
          "hmph hydrolyze apud well-groomed notwithstanding glaring triumphantly irresponsible numeric soybean",
        name: "<value>",
        accountCode: "<value>",
        accountId: "<id>",
        dimensions: [],
        discountItemPercentage: 2334.11,
      },
    ],
    discountPercentage: 7307.77,
    shippingType: "DELIVERY",
    shippingDate: "<value>",
    shippingEndDate: "<value>",
    lineAmountTypes: "EXCLUSIVE",
    dueDate: "<value>",
    paidDate: "<value>",
    paymentTermDuration: 968.76,
  },
};
```

## Fields

| Field                                                                      | Type                                                                       | Required                                                                   | Description                                                                |
| -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| `invoiceId`                                                                | *string*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `environmentName`                                                          | *string*                                                                   | :heavy_minus_sign:                                                         | N/A                                                                        |
| `companyId`                                                                | *string*                                                                   | :heavy_minus_sign:                                                         | N/A                                                                        |
| `xApiKey`                                                                  | *string*                                                                   | :heavy_minus_sign:                                                         | API key                                                                    |
| `xAccountKey`                                                              | *string*                                                                   | :heavy_minus_sign:                                                         | Account key                                                                |
| `body`                                                                     | [models.PatchInvoiceRequestDto](../../models/patch-invoice-request-dto.md) | :heavy_check_mark:                                                         | N/A                                                                        |