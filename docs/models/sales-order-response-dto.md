# SalesOrderResponseDto

## Example Usage

```typescript
import { SalesOrderResponseDto } from "@maesn/typescript-sdk/models";

let value: SalesOrderResponseDto = {
  id: "<id>",
  addresses: null,
  billingContactId: "<id>",
  comment:
    "Carbonite web goalkeeper gloves are ergonomically designed to give easy fit",
  contactId: "<id>",
  createdDate: "<value>",
  currency: "Dobra",
  deliveryDate: "<value>",
  lineItems: [],
  orderDate: null,
  projectId: "<id>",
  shippingContactId: null,
  status: "OPEN",
  taskId: "<id>",
  totalDiscountAmount: 9876.8,
  totalDiscountPercentage: 3789.05,
  totalGrossAmount: 93.06,
  totalNetAmount: 3568.42,
  totalTaxAmount: 883.63,
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                     | Type                                                                                      | Required                                                                                  | Description                                                                               |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `id`                                                                                      | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `addresses`                                                                               | [models.Address](../models/address.md)[]                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `billingContactId`                                                                        | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `comment`                                                                                 | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `contactId`                                                                               | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `createdDate`                                                                             | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `currency`                                                                                | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `deliveryDate`                                                                            | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `lineItems`                                                                               | [models.SalesOrderLineItemResponseDto](../models/sales-order-line-item-response-dto.md)[] | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `oneLineAddress`                                                                          | *string*                                                                                  | :heavy_minus_sign:                                                                        | N/A                                                                                       |
| `orderDate`                                                                               | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `projectId`                                                                               | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `shippingContactId`                                                                       | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `status`                                                                                  | [models.SalesOrderResponseDtoStatus](../models/sales-order-response-dto-status.md)        | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `taskId`                                                                                  | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `totalDiscountAmount`                                                                     | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `totalDiscountPercentage`                                                                 | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `totalGrossAmount`                                                                        | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `totalNetAmount`                                                                          | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `totalTaxAmount`                                                                          | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `updatedDate`                                                                             | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |