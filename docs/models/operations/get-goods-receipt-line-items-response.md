# GetGoodsReceiptLineItemsResponse

## Example Usage

```typescript
import { GetGoodsReceiptLineItemsResponse } from "maesn/models/operations";

let value: GetGoodsReceiptLineItemsResponse = {
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
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                          | Type                                                                                                           | Required                                                                                                       | Description                                                                                                    |
| -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                         | [models.MetaResponse](../../models/meta-response.md)                                                           | :heavy_check_mark:                                                                                             | N/A                                                                                                            |
| `data`                                                                                                         | [models.GoodsReceiptLineItemResponse](../../models/goods-receipt-line-item-response.md)[]                      | :heavy_check_mark:                                                                                             | N/A                                                                                                            |
| `errors`                                                                                                       | [operations.GetGoodsReceiptLineItemsErrors](../../models/operations/get-goods-receipt-line-items-errors.md)    | :heavy_check_mark:                                                                                             | N/A                                                                                                            |
| `rawData`                                                                                                      | [operations.GetGoodsReceiptLineItemsRawData](../../models/operations/get-goods-receipt-line-items-raw-data.md) | :heavy_check_mark:                                                                                             | N/A                                                                                                            |