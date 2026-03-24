# PatchInvoiceRequestDto

## Example Usage

```typescript
import { PatchInvoiceRequestDto } from "maesn/models";

let value: PatchInvoiceRequestDto = {
  invoiceId: "<id>",
  contactId: "<id>",
  name: "<value>",
  reference: "<value>",
  currency: "Uzbekistan Sum",
  invoiceDate: "<value>",
  journalCode: "<value>",
  paymentTermId: "<id>",
  fileId: "<id>",
  status: "DRAFT",
  invoiceType: "STANDARD",
  oneLineAddress: "<value>",
  addresses: [],
  taxRule: "EXTERNALSERVICE",
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
  discountPercentage: 2968.75,
  shippingType: "DELIVERY",
  shippingDate: "<value>",
  shippingEndDate: "<value>",
  lineAmountTypes: "INCLUSIVE",
  dueDate: "<value>",
  paidDate: "<value>",
  paymentTermDuration: 823.72,
};
```

## Fields

| Field                                                                                                    | Type                                                                                                     | Required                                                                                                 | Description                                                                                              |
| -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| `invoiceId`                                                                                              | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `contactId`                                                                                              | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `name`                                                                                                   | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `reference`                                                                                              | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `currency`                                                                                               | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `invoiceDate`                                                                                            | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `journalCode`                                                                                            | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `paymentTermId`                                                                                          | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `fileId`                                                                                                 | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `status`                                                                                                 | [models.PatchInvoiceRequestDtoStatus](../models/patch-invoice-request-dto-status.md)                     | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `invoiceType`                                                                                            | [models.PatchInvoiceRequestDtoInvoiceType](../models/patch-invoice-request-dto-invoice-type.md)          | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `oneLineAddress`                                                                                         | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `addresses`                                                                                              | [models.Address](../models/address.md)[]                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `taxRule`                                                                                                | [models.PatchInvoiceRequestDtoTaxRule](../models/patch-invoice-request-dto-tax-rule.md)                  | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `taxText`                                                                                                | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `lineItems`                                                                                              | [models.PatchLineItemRequest](../models/patch-line-item-request.md)[]                                    | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `discountPercentage`                                                                                     | *number*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `shippingType`                                                                                           | [models.PatchInvoiceRequestDtoShippingType](../models/patch-invoice-request-dto-shipping-type.md)        | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `shippingDate`                                                                                           | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `shippingEndDate`                                                                                        | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `lineAmountTypes`                                                                                        | [models.PatchInvoiceRequestDtoLineAmountTypes](../models/patch-invoice-request-dto-line-amount-types.md) | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `dueDate`                                                                                                | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `paidDate`                                                                                               | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `paymentTermDuration`                                                                                    | *number*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |