# PurchaseOrderResponseDto

## Example Usage

```typescript
import { PurchaseOrderResponseDto } from "@maesn/typescript-sdk/models";

let value: PurchaseOrderResponseDto = {
  id: null,
  addresses: [
    {},
  ],
  approvalDate: "<value>",
  comment:
    "Andy shoes are designed to keeping in mind durability as well as trends, the most stylish range of shoes & sandals",
  createdDate: "<value>",
  currency: "MXN",
  description: "deserted disappointment which graceful nautical",
  lineItems: [
    {
      id: "<id>",
      itemId: "<id>",
      createdDate: "<value>",
      description: "zen zowie where before anti wearily",
      itemName: "<value>",
      quantity: 7516.64,
      taxCode: "<value>",
      taxRatePercentage: 1922.59,
      totalDiscountAmount: 6117.6,
      totalDiscountPercentage: 3161.7,
      totalGrossAmount: 9740.85,
      totalNetAmount: 3615.75,
      totalTaxAmount: 980.25,
      unitAmount: 8062.11,
      unitDiscountAmount: null,
      unitDiscountPercentage: 5376.51,
      unitName: "<value>",
      updatedDate: "<value>",
    },
  ],
  orderDate: "<value>",
  paymentTermId: "<id>",
  reference: null,
  status: "CLOSED",
  supplierId: "<id>",
  totalDiscountAmount: null,
  totalDiscountPercentage: 7320.67,
  totalGrossAmount: 5696.42,
  totalNetAmount: 9018.05,
  totalTaxAmount: 3118.75,
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `id`                                                                                            | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `addresses`                                                                                     | [models.Address](../models/address.md)[]                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `approvalDate`                                                                                  | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `comment`                                                                                       | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `createdDate`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `currency`                                                                                      | [models.PurchaseOrderResponseDtoCurrency](../models/purchase-order-response-dto-currency.md)    | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `description`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `lineItems`                                                                                     | [models.PurchaseOrderLineItemResponseDto](../models/purchase-order-line-item-response-dto.md)[] | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `orderDate`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paymentTermId`                                                                                 | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `reference`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `status`                                                                                        | [models.PurchaseOrderResponseDtoStatus](../models/purchase-order-response-dto-status.md)        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `supplierId`                                                                                    | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalDiscountAmount`                                                                           | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalDiscountPercentage`                                                                       | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalGrossAmount`                                                                              | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalNetAmount`                                                                                | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalTaxAmount`                                                                                | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `updatedDate`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |