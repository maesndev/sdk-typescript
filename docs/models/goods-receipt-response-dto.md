# GoodsReceiptResponseDto

## Example Usage

```typescript
import { GoodsReceiptResponseDto } from "maesn/models";

let value: GoodsReceiptResponseDto = {
  id: "<id>",
  comment:
    "Carbonite web goalkeeper gloves are ergonomically designed to give easy fit",
  createdDate: "<value>",
  description: "um boo phew versus tomorrow stealthily gadzooks plan whether",
  lineItems: [
    {
      id: "<id>",
      createdDate: "<value>",
      description:
        "vastly reprimand uh-huh restfully unto quietly yieldingly recklessly insignificant",
      itemId: "<id>",
      itemName: "<value>",
      projectId: "<id>",
      purchaseOrderId: "<id>",
      quantityOrdered: 7685.77,
      quantityReceived: 725.02,
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