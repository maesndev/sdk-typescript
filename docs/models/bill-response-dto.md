# BillResponseDto

## Example Usage

```typescript
import { BillResponseDto } from "@maesn/typescript-sdk/models";

let value: BillResponseDto = {
  id: "<id>",
  accountId: "<id>",
  addresses: null,
  billDate: "<value>",
  billNumber: "<value>",
  contactId: "<id>",
  createdDate: "<value>",
  currency: "Falkland Islands Pound",
  deliveryDate: "<value>",
  dueDate: "<value>",
  fileId: "<id>",
  journalCode: "<value>",
  lineItems: [
    {
      id: "<id>",
      accountId: null,
      accountNumber: "<value>",
      createdDate: "<value>",
      deferredEndDate: "<value>",
      deferredStartDate: "<value>",
      description: "oof dish ouch rotten mortar giant",
      dimensions: [],
      itemId: "<id>",
      itemName: "<value>",
      quantity: 8319.09,
      taxCode: "<value>",
      taxRatePercentage: 4598.12,
      totalDiscountAmount: 7548.91,
      totalDiscountPercentage: 5308.45,
      totalGrossAmount: 5588.18,
      totalNetAmount: 1273.27,
      totalTaxAmount: 7450.14,
      unitAmount: 4776.62,
      unitDiscountAmount: 6000.9,
      unitDiscountPercentage: 4093.91,
      unitName: "<value>",
      updatedDate: "<value>",
    },
  ],
  name: "<value>",
  oneLineAddress: null,
  paidDate: "<value>",
  paymentTermCode: "<value>",
  paymentStatus: "UNKNOWN",
  paymentDays: 2097.58,
  reference: "<value>",
  shippingDate: "<value>",
  shippingType: "SERVICE_PERIOD",
  status: "CORRECTIVE",
  taxRule: "PHOTOVOLTAIC_EQUIPMENT",
  taxText: "<value>",
  totalDiscountAmount: 1067.58,
  totalDiscountPercentage: 1018.42,
  totalGrossAmount: null,
  totalNetAmount: null,
  totalTaxAmount: 5862.61,
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                | Type                                                                                 | Required                                                                             | Description                                                                          |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| `id`                                                                                 | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `accountId`                                                                          | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `addresses`                                                                          | [models.Address](../models/address.md)[]                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `billDate`                                                                           | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `billNumber`                                                                         | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `contactId`                                                                          | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `createdDate`                                                                        | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `currency`                                                                           | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `deliveryDate`                                                                       | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `dueDate`                                                                            | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `fileId`                                                                             | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `journalCode`                                                                        | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `lineItems`                                                                          | [models.BillLineItemResponseDto](../models/bill-line-item-response-dto.md)[]         | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `name`                                                                               | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `oneLineAddress`                                                                     | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `paidDate`                                                                           | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `paymentTermCode`                                                                    | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `paymentStatus`                                                                      | [models.BillResponseDtoPaymentStatus](../models/bill-response-dto-payment-status.md) | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `paymentDays`                                                                        | *number*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `reference`                                                                          | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `shippingDate`                                                                       | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `shippingType`                                                                       | [models.BillResponseDtoShippingType](../models/bill-response-dto-shipping-type.md)   | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `status`                                                                             | [models.BillResponseDtoStatus](../models/bill-response-dto-status.md)                | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `taxRule`                                                                            | [models.BillResponseDtoTaxRule](../models/bill-response-dto-tax-rule.md)             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `taxText`                                                                            | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `totalDiscountAmount`                                                                | *number*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `totalDiscountPercentage`                                                            | *number*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `totalGrossAmount`                                                                   | *number*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `totalNetAmount`                                                                     | *number*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `totalTaxAmount`                                                                     | *number*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `updatedDate`                                                                        | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |