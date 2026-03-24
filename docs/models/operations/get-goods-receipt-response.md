# GetGoodsReceiptResponse

## Example Usage

```typescript
import { GetGoodsReceiptResponse } from "maesn/models/operations";

let value: GetGoodsReceiptResponse = {
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
  data: {
    id: "<id>",
    comment:
      "The beautiful range of Apple Naturalé that has an exciting mix of natural ingredients. With the Goodness of 100% Natural Ingredients",
    createdDate: "<value>",
    description: "athwart gigantic into yum",
    lineItems: [],
    reference: "<value>",
    supplierId: "<id>",
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `meta`                                                                                     | [models.MetaResponse](../../models/meta-response.md)                                       | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.GoodsReceiptResponseDto](../../models/goods-receipt-response-dto.md)               | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.GetGoodsReceiptErrors](../../models/operations/get-goods-receipt-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.GetGoodsReceiptRawData](../../models/operations/get-goods-receipt-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |