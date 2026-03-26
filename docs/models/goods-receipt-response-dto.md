# GoodsReceiptResponseDto

## Example Usage

```typescript
import { GoodsReceiptResponseDto } from "@maesn/typescript-sdk/models";

let value: GoodsReceiptResponseDto = {
  id: "<id>",
  comment:
    "New ABC 13 9370, 13.3, 5th Gen CoreA5-8250U, 8GB RAM, 256GB SSD, power UHD Graphics, OS 10 Home, OS Office A & J 2016",
  createdDate: "<value>",
  description: null,
  lineItems: [
    {
      id: "<id>",
      createdDate: "<value>",
      description: "kielbasa sunbeam against",
      itemId: "<id>",
      itemName: "<value>",
      projectId: "<id>",
      purchaseOrderId: "<id>",
      quantityOrdered: 9504.4,
      quantityReceived: 1980.42,
      updatedDate: "<value>",
    },
  ],
  reference: "<value>",
  supplierId: "<id>",
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `id`                                                                                   | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `comment`                                                                              | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `createdDate`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `description`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `lineItems`                                                                            | [models.GoodsReceiptLineItemResponse](../models/goods-receipt-line-item-response.md)[] | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `reference`                                                                            | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `supplierId`                                                                           | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `updatedDate`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |