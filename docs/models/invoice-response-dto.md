# InvoiceResponseDto

## Example Usage

```typescript
import { InvoiceResponseDto } from "@maesn/typescript-sdk/models";

let value: InvoiceResponseDto = {
  id: "<id>",
  invoiceId: "<id>",
  addresses: [],
  contactId: "<id>",
  createdDate: "<value>",
  currency: "Yemeni Rial",
  discountAmount: 3256.21,
  dueDate: "<value>",
  invoiceDate: "<value>",
  invoiceNumber: "<value>",
  invoiceType: null,
  journalCode: "<value>",
  lineAmountTypes: null,
  lineItems: [
    {
      lineItemId: "<id>",
      accountId: "<id>",
      createdDate: "<value>",
      description: "atrium worth strange frequent wallop though barring both",
      dimensions: [
        {
          id: "<id>",
          categoryName: "<value>",
          name: "<value>",
        },
      ],
      discountItemAmount: 1191.85,
      discountItemPercentage: 4359.97,
      grossAmount: 9843.51,
      itemsAmount: 6379.48,
      itemId: null,
      name: "<value>",
      quantity: 8171.72,
      taxRatePercentage: 1753.39,
      unitAmount: 5556.99,
      updatedDate: null,
    },
  ],
  name: "<value>",
  oneLineAddress: "<value>",
  paidDate: "<value>",
  paymentStatus: "CREDIT_NOTE_CLEARED",
  paymentTermDuration: 716.86,
  paymentTermId: "<id>",
  reference: "<value>",
  shippingDate: "<value>",
  status: "OVERDUE",
  sumNetAmount: 2893.98,
  taxRule: "SMALL_BUSINESS_EXEMPTION",
  totalAmount: 4785.28,
  totalTaxAmount: 7256.01,
  updatedDate: null,
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `id`                                                                                            | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `invoiceId`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `addresses`                                                                                     | [models.Address](../models/address.md)[]                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `contactId`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `createdDate`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `currency`                                                                                      | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `discountAmount`                                                                                | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `dueDate`                                                                                       | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `fileId`                                                                                        | *string*                                                                                        | :heavy_minus_sign:                                                                              | N/A                                                                                             |
| `invoiceDate`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `invoiceNumber`                                                                                 | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `invoiceType`                                                                                   | [models.InvoiceResponseDtoInvoiceType](../models/invoice-response-dto-invoice-type.md)          | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `journalCode`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `lineAmountTypes`                                                                               | [models.InvoiceResponseDtoLineAmountTypes](../models/invoice-response-dto-line-amount-types.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `lineItems`                                                                                     | [models.LineItemResponseDto](../models/line-item-response-dto.md)[]                             | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `name`                                                                                          | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `oneLineAddress`                                                                                | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paidDate`                                                                                      | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paymentStatus`                                                                                 | [models.InvoiceResponseDtoPaymentStatus](../models/invoice-response-dto-payment-status.md)      | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paymentTermDuration`                                                                           | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paymentTermId`                                                                                 | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `reference`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `shippingDate`                                                                                  | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `status`                                                                                        | [models.InvoiceResponseDtoStatus](../models/invoice-response-dto-status.md)                     | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `sumNetAmount`                                                                                  | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `taxRule`                                                                                       | [models.InvoiceResponseDtoTaxRule](../models/invoice-response-dto-tax-rule.md)                  | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalAmount`                                                                                   | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalTaxAmount`                                                                                | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `updatedDate`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |