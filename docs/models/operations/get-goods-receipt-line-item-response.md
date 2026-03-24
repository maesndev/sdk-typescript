# GetGoodsReceiptLineItemResponse

## Example Usage

```typescript
import { GetGoodsReceiptLineItemResponse } from "maesn/models/operations";

let value: GetGoodsReceiptLineItemResponse = {
  meta: {
    warnings: [
      "<value 1>",
      "<value 2>",
    ],
    pagination: {
      total: 3438.77,
      perPage: 5109.63,
      currentPage: 2626.79,
      totalPages: 3561.84,
    },
  },
  data: [
    {
      id: "<id>",
      createdDate: "<value>",
      description: "showy perspire overcoat record drat",
      itemId: "<id>",
      itemName: "<value>",
      projectId: "<id>",
      purchaseOrderId: "<id>",
      quantityOrdered: 3598.11,
      quantityReceived: 251.22,
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                        | Type                                                                                                         | Required                                                                                                     | Description                                                                                                  |
| ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| `meta`                                                                                                       | [models.MetaResponse](../../models/meta-response.md)                                                         | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `data`                                                                                                       | [models.GoodsReceiptLineItemResponse](../../models/goods-receipt-line-item-response.md)[]                    | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `errors`                                                                                                     | [operations.GetGoodsReceiptLineItemErrors](../../models/operations/get-goods-receipt-line-item-errors.md)    | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `rawData`                                                                                                    | [operations.GetGoodsReceiptLineItemRawData](../../models/operations/get-goods-receipt-line-item-raw-data.md) | :heavy_check_mark:                                                                                           | N/A                                                                                                          |