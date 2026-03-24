# BillResponseDto

## Example Usage

```typescript
import { BillResponseDto } from "maesn/models";

let value: BillResponseDto = {
  id: "<id>",
  accountId: "<id>",
  addresses: [],
  billDate: "<value>",
  billNumber: "<value>",
  contactId: "<id>",
  createdDate: {},
  currency: "Belize Dollar",
  deliveryDate: "<value>",
  dueDate: "<value>",
  fileId: "<id>",
  journalCode: "<value>",
  lineItems: [],
  name: "<value>",
  oneLineAddress: "<value>",
  paidDate: {},
  paymentTermCode: "<value>",
  paymentStatus: "CREDIT_NOTE_CLEARED",
  paymentDays: 6948.49,
  reference: "<value>",
  shippingDate: {},
  shippingType: "SERVICE",
  status: "PARTIALLY_OVERDUE",
  taxRule: "INTRACOMMUNITY_GOODS",
  taxText: "<value>",
  totalDiscountAmount: 2812.88,
  totalDiscountPercentage: 4522.96,
  totalGrossAmount: 7426.74,
  totalNetAmount: 4741.69,
  totalTaxAmount: 5285.58,
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
| `createdDate`                                                                        | [models.BillResponseDtoCreatedDate](../models/bill-response-dto-created-date.md)     | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `currency`                                                                           | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `deliveryDate`                                                                       | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `dueDate`                                                                            | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `fileId`                                                                             | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `journalCode`                                                                        | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `lineItems`                                                                          | [models.BillLineItemResponseDto](../models/bill-line-item-response-dto.md)[]         | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `name`                                                                               | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `oneLineAddress`                                                                     | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `paidDate`                                                                           | [models.BillResponseDtoPaidDate](../models/bill-response-dto-paid-date.md)           | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `paymentTermCode`                                                                    | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `paymentStatus`                                                                      | [models.BillResponseDtoPaymentStatus](../models/bill-response-dto-payment-status.md) | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `paymentDays`                                                                        | *number*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `reference`                                                                          | *string*                                                                             | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `shippingDate`                                                                       | [models.BillResponseDtoShippingDate](../models/bill-response-dto-shipping-date.md)   | :heavy_check_mark:                                                                   | N/A                                                                                  |
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