# InvoiceResponseDto

## Example Usage

```typescript
import { InvoiceResponseDto } from "maesn/models";

let value: InvoiceResponseDto = {
  invoiceId: "<id>",
  addresses: [],
  contactId: "<id>",
  createdDate: {},
  currency: "Mauritius Rupee",
  discountAmount: 3722.61,
  dueDate: {},
  fileId: "<id>",
  invoiceDate: {},
  invoiceNumber: "<value>",
  invoiceType: "STANDARD",
  journalCode: "<value>",
  lineAmountTypes: "EXCLUSIVE",
  lineItems: [],
  name: "<value>",
  oneLineAddress: "<value>",
  paidDate: {},
  paymentStatus: "DEBITED",
  paymentTermDuration: 9612.08,
  paymentTermId: "<id>",
  reference: "<value>",
  shippingDate: {},
  status: "PAID",
  sumNetAmount: 3256.21,
  taxRule: "OSS_SERVICES",
  totalAmount: 1379.67,
  totalTaxAmount: 2490.46,
  updatedDate: {},
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `invoiceId`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `addresses`                                                                                     | [models.Address](../models/address.md)[]                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `contactId`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `createdDate`                                                                                   | [models.InvoiceResponseDtoCreatedDate](../models/invoice-response-dto-created-date.md)          | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `currency`                                                                                      | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `discountAmount`                                                                                | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `dueDate`                                                                                       | [models.DueDate](../models/due-date.md)                                                         | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `fileId`                                                                                        | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `invoiceDate`                                                                                   | [models.InvoiceDate](../models/invoice-date.md)                                                 | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `invoiceNumber`                                                                                 | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `invoiceType`                                                                                   | [models.InvoiceResponseDtoInvoiceType](../models/invoice-response-dto-invoice-type.md)          | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `journalCode`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `lineAmountTypes`                                                                               | [models.InvoiceResponseDtoLineAmountTypes](../models/invoice-response-dto-line-amount-types.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `lineItems`                                                                                     | [models.LineItemResponseDto](../models/line-item-response-dto.md)[]                             | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `name`                                                                                          | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `oneLineAddress`                                                                                | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paidDate`                                                                                      | [models.InvoiceResponseDtoPaidDate](../models/invoice-response-dto-paid-date.md)                | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paymentStatus`                                                                                 | [models.InvoiceResponseDtoPaymentStatus](../models/invoice-response-dto-payment-status.md)      | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paymentTermDuration`                                                                           | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paymentTermId`                                                                                 | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `reference`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `shippingDate`                                                                                  | [models.InvoiceResponseDtoShippingDate](../models/invoice-response-dto-shipping-date.md)        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `status`                                                                                        | [models.InvoiceResponseDtoStatus](../models/invoice-response-dto-status.md)                     | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `sumNetAmount`                                                                                  | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `taxRule`                                                                                       | [models.InvoiceResponseDtoTaxRule](../models/invoice-response-dto-tax-rule.md)                  | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalAmount`                                                                                   | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalTaxAmount`                                                                                | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `updatedDate`                                                                                   | [models.InvoiceResponseDtoUpdatedDate](../models/invoice-response-dto-updated-date.md)          | :heavy_check_mark:                                                                              | N/A                                                                                             |