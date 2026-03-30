# GetGoodsReceiptLineItemResponse

Goods receipt line item record matching the provided ID

## Example Usage

```typescript
import { GetGoodsReceiptLineItemResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetGoodsReceiptLineItemResponse = {
  data: {
    id: "<id>",
    createdDate: "<value>",
    description: "skateboard airport since bravely aboard",
    itemId: "<id>",
    itemName: "<value>",
    projectId: null,
    purchaseOrderId: "<id>",
    quantityOrdered: null,
    quantityReceived: 1638.32,
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                        | Type                                                                                                         | Required                                                                                                     | Description                                                                                                  |
| ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| `meta`                                                                                                       | [operations.GetGoodsReceiptLineItemMeta](../../models/operations/get-goods-receipt-line-item-meta.md)        | :heavy_minus_sign:                                                                                           | N/A                                                                                                          |
| `data`                                                                                                       | [models.GoodsReceiptLineItemResponse](../../models/goods-receipt-line-item-response.md)                      | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `errors`                                                                                                     | [operations.GetGoodsReceiptLineItemErrors](../../models/operations/get-goods-receipt-line-item-errors.md)    | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `rawData`                                                                                                    | [operations.GetGoodsReceiptLineItemRawData](../../models/operations/get-goods-receipt-line-item-raw-data.md) | :heavy_check_mark:                                                                                           | N/A                                                                                                          |