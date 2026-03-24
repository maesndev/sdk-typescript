# SalesOrderResponseDto

## Example Usage

```typescript
import { SalesOrderResponseDto } from "maesn/models";

let value: SalesOrderResponseDto = {
  id: "<id>",
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
    "Andy shoes are designed to keeping in mind durability as well as trends, the most stylish range of shoes & sandals",
  contactId: "<id>",
  createdDate: "<value>",
  currency: "Peso Uruguayo",
  deliveryDate: "<value>",
  lineItems: [],
  oneLineAddress: "<value>",
  orderDate: "<value>",
  projectId: "<id>",
  shippingContactId: "<id>",
  status: "DRAFT",
  taskId: "<id>",
  totalDiscountAmount: 4434.31,
  totalDiscountPercentage: 3511.34,
  totalGrossAmount: 2886.79,
  totalNetAmount: 7995.07,
  totalTaxAmount: 9789.92,
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
| `oneLineAddress`                                                                          | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
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