# CreateSalesOrderRequestDto

## Example Usage

```typescript
import { CreateSalesOrderRequestDto } from "maesn/models";

let value: CreateSalesOrderRequestDto = {
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
  billingContactId: "<id>",
  comment:
    "Ergonomic executive chair upholstered in bonded black leather and PVC padded seat and back for all-day comfort and support",
  contactId: "<id>",
  currency: "Comoro Franc",
  deliveryDate: "<value>",
  lineItems: [
    {
      itemId: "<id>",
      description: "in by overload till well-worn clearly",
      itemName: "<value>",
      quantity: 5511.07,
      taxCode: "<value>",
      taxRatePercentage: 9975.5,
      totalDiscountAmount: 8832.07,
      totalDiscountPercentage: 9257.51,
      totalGrossAmount: 4200.1,
      totalNetAmount: 644.06,
      totalTaxAmount: 7970.48,
      unitAmount: 166.34,
      unitDiscountAmount: 1720.34,
      unitDiscountPercentage: 7835.61,
      unitName: "<value>",
    },
  ],
  oneLineAddress: "<value>",
  orderDate: "<value>",
  projectId: "<id>",
  shippingContactId: "<id>",
  status: "OPEN",
  totalDiscountAmount: 5667.52,
  totalDiscountPercentage: 7673.78,
  totalGrossAmount: 211.13,
  totalNetAmount: 624.56,
  totalTaxAmount: 3833.2,
  version: "<value>",
};
```

## Fields

| Field                                                                                                | Type                                                                                                 | Required                                                                                             | Description                                                                                          |
| ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| `addresses`                                                                                          | [models.Address](../models/address.md)[]                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `billingContactId`                                                                                   | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `comment`                                                                                            | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `contactId`                                                                                          | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `currency`                                                                                           | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `deliveryDate`                                                                                       | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `lineItems`                                                                                          | [models.CreateSalesOrderLineItemRequestDto](../models/create-sales-order-line-item-request-dto.md)[] | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `oneLineAddress`                                                                                     | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `orderDate`                                                                                          | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `projectId`                                                                                          | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `shippingContactId`                                                                                  | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `status`                                                                                             | [models.CreateSalesOrderRequestDtoStatus](../models/create-sales-order-request-dto-status.md)        | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `totalDiscountAmount`                                                                                | *number*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `totalDiscountPercentage`                                                                            | *number*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `totalGrossAmount`                                                                                   | *number*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `totalNetAmount`                                                                                     | *number*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `totalTaxAmount`                                                                                     | *number*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `version`                                                                                            | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |