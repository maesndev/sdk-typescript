# CreateInvoiceRequestDto

## Example Usage

```typescript
import { CreateInvoiceRequestDto } from "maesn/models";

let value: CreateInvoiceRequestDto = {
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
  currency: "CFA Franc BCEAO",
  discountPercentage: 5088.56,
  dueDate: "<value>",
  fileId: "<id>",
  grossTotalAmount: 4524.68,
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
  paymentTermDuration: 4645.83,
  paymentTermId: "<id>",
  reference: "<value>",
  shippingDate: "<value>",
  shippingType: "NONE",
  shippingEndDate: "<value>",
  status: "PARTIALLY_PAID",
  taxRule: "OSS_GOODS",
  taxText: "<value>",
};
```

## Fields

| Field                                                                                               | Type                                                                                                | Required                                                                                            | Description                                                                                         |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `invoiceId`                                                                                         | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `addresses`                                                                                         | [models.Address](../models/address.md)[]                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `contactId`                                                                                         | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `currency`                                                                                          | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `discountPercentage`                                                                                | *number*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `dueDate`                                                                                           | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `fileId`                                                                                            | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `grossTotalAmount`                                                                                  | *number*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `invoiceDate`                                                                                       | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `invoiceNumber`                                                                                     | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `invoiceType`                                                                                       | [models.CreateInvoiceRequestDtoInvoiceType](../models/create-invoice-request-dto-invoice-type.md)   | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `journalCode`                                                                                       | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `lineAmountTypes`                                                                                   | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `lineItems`                                                                                         | [models.CreateLineItemRequestDto](../models/create-line-item-request-dto.md)[]                      | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `name`                                                                                              | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `oneLineAddress`                                                                                    | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `paidDate`                                                                                          | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `paymentTermDuration`                                                                               | *number*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `paymentTermId`                                                                                     | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `reference`                                                                                         | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `shippingDate`                                                                                      | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `shippingType`                                                                                      | [models.CreateInvoiceRequestDtoShippingType](../models/create-invoice-request-dto-shipping-type.md) | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `shippingEndDate`                                                                                   | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `status`                                                                                            | [models.CreateInvoiceRequestDtoStatus](../models/create-invoice-request-dto-status.md)              | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `taxRule`                                                                                           | [models.CreateInvoiceRequestDtoTaxRule](../models/create-invoice-request-dto-tax-rule.md)           | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `taxText`                                                                                           | *string*                                                                                            | :heavy_check_mark:                                                                                  | N/A                                                                                                 |