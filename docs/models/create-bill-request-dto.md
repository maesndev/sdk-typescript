# CreateBillRequestDto

## Example Usage

```typescript
import { CreateBillRequestDto } from "maesn/models";

let value: CreateBillRequestDto = {
  accountId: "<id>",
  addresses: [],
  billDate: "<value>",
  billNumber: "<value>",
  contactId: "<id>",
  currency: "Manat",
  deliveryDate: "<value>",
  dueDate: "<value>",
  fileId: "<id>",
  journalCode: "<value>",
  lineItems: [
    {
      id: "<id>",
      accountId: "<id>",
      accountNumber: "<value>",
      deferredEndDate: "<value>",
      deferredStartDate: "<value>",
      description:
        "whose sedately zowie soon yowza solemnly step-mother painfully phooey",
      dimensions: [],
      itemId: "<id>",
      itemName: "<value>",
      quantity: 5519.84,
      taxCode: "<value>",
      taxRatePercentage: 4194.04,
      totalDiscountAmount: 2979.82,
      totalDiscountPercentage: 6926.8,
      totalGrossAmount: 9233.58,
      totalNetAmount: 1233.01,
      totalTaxAmount: 8119.37,
      unitAmount: 4907.85,
      unitDiscountAmount: 1684.91,
      unitDiscountPercentage: 9320.51,
      unitName: "<value>",
    },
  ],
  name: "<value>",
  oneLineAddress: "<value>",
  paidDate: {},
  paymentTermCode: "<value>",
  paymentStatus: "PARTLY_PAID",
  paymentDays: 2283.7,
  reference: "<value>",
  shippingDate: {},
  shippingType: "SERVICE",
  status: "OVERDUE",
  taxRule: "PHOTOVOLTAIC_EQUIPMENT",
  taxText: "<value>",
  totalDiscountAmount: 4762.73,
  totalDiscountPercentage: 7548.08,
  totalGrossAmount: 8439,
  totalNetAmount: 2390.82,
  totalTaxAmount: 5759.04,
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `accountId`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `addresses`                                                                                     | [models.Address](../models/address.md)[]                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `billDate`                                                                                      | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `billNumber`                                                                                    | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `contactId`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `currency`                                                                                      | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `deliveryDate`                                                                                  | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `dueDate`                                                                                       | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `fileId`                                                                                        | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `journalCode`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `lineItems`                                                                                     | [models.CreateBillLineItemRequestDto](../models/create-bill-line-item-request-dto.md)[]         | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `name`                                                                                          | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `oneLineAddress`                                                                                | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paidDate`                                                                                      | [models.CreateBillRequestDtoPaidDate](../models/create-bill-request-dto-paid-date.md)           | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paymentTermCode`                                                                               | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paymentStatus`                                                                                 | [models.CreateBillRequestDtoPaymentStatus](../models/create-bill-request-dto-payment-status.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paymentDays`                                                                                   | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `reference`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `shippingDate`                                                                                  | [models.CreateBillRequestDtoShippingDate](../models/create-bill-request-dto-shipping-date.md)   | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `shippingType`                                                                                  | [models.CreateBillRequestDtoShippingType](../models/create-bill-request-dto-shipping-type.md)   | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `status`                                                                                        | [models.CreateBillRequestDtoStatus](../models/create-bill-request-dto-status.md)                | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `taxRule`                                                                                       | [models.CreateBillRequestDtoTaxRule](../models/create-bill-request-dto-tax-rule.md)             | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `taxText`                                                                                       | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalDiscountAmount`                                                                           | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalDiscountPercentage`                                                                       | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalGrossAmount`                                                                              | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalNetAmount`                                                                                | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalTaxAmount`                                                                                | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |