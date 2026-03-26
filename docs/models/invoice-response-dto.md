# InvoiceResponseDto

## Example Usage

```typescript
import { InvoiceResponseDto } from "@maesn/typescript-sdk/models";

let value: InvoiceResponseDto = {
  invoiceId: "<id>",
  addresses: [],
  contactId: "<id>",
  createdDate: "<value>",
  currency: "Rupiah",
  discountAmount: 6540.46,
  dueDate: "<value>",
  invoiceDate: "<value>",
  invoiceNumber: "<value>",
  invoiceType: "STANDARD",
  journalCode: "<value>",
  lineAmountTypes: null,
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
  paymentStatus: "BAD_DEBT",
  paymentTermDuration: 5046.51,
  paymentTermId: "<id>",
  reference: null,
  shippingDate: "<value>",
  status: "DRAFT",
  sumNetAmount: null,
  taxRule: "SMALL_BUSINESS_EXEMPTION",
  totalAmount: null,
  totalTaxAmount: 1490.41,
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
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