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
  fileId: "<id>",
  invoiceDate: "<value>",
  invoiceNumber: null,
  invoiceType: "STANDARD",
  journalCode: "<value>",
  lineAmountTypes: "EXCLUSIVE",
  lineItems: [
    {
      lineItemId: "<id>",
      accountId: "<id>",
      createdDate: "<value>",
      description: "sheepishly poppy overcooked commercial opposite",
      dimensions: [],
      discountItemAmount: 6563.83,
      discountItemPercentage: 2599.87,
      grossAmount: 47.73,
      itemsAmount: 850.68,
      itemId: "<id>",
      name: "<value>",
      quantity: 2497.18,
      taxCode: "<value>",
      taxRatePercentage: 7472.13,
      unitAmount: null,
      updatedDate: "<value>",
    },
  ],
  name: "<value>",
  oneLineAddress: "<value>",
  paidDate: "<value>",
  paymentStatus: "DEBITED",
  paymentTermDuration: 9843.51,
  paymentTermId: "<id>",
  reference: "<value>",
  salesOrderId: null,
  shippingDate: "<value>",
  status: "OVERDUE",
  sumNetAmount: 1753.39,
  taxRule: "CONSTRUCTION_SERVICE",
  totalAmount: null,
  totalTaxAmount: 2516,
  updatedDate: "<value>",
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
| `fileId`                                                                                        | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
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
| `salesOrderId`                                                                                  | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `shippingDate`                                                                                  | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `status`                                                                                        | [models.InvoiceResponseDtoStatus](../models/invoice-response-dto-status.md)                     | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `sumNetAmount`                                                                                  | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `taxRule`                                                                                       | [models.InvoiceResponseDtoTaxRule](../models/invoice-response-dto-tax-rule.md)                  | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalAmount`                                                                                   | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalTaxAmount`                                                                                | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `updatedDate`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |