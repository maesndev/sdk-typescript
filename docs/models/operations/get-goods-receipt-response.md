# GetGoodsReceiptResponse

## Example Usage

```typescript
import { GetGoodsReceiptResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetGoodsReceiptResponse = {
  data: {
    id: "<id>",
    comment:
      "The Apollotech B340 is an affordable wireless mouse with reliable connectivity, 12 months battery life and modern design",
    createdDate: "<value>",
    description: null,
    lineItems: null,
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
| `meta`                                                                                     | [operations.GetGoodsReceiptMeta](../../models/operations/get-goods-receipt-meta.md)        | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.GoodsReceiptResponseDto](../../models/goods-receipt-response-dto.md)               | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.GetGoodsReceiptErrors](../../models/operations/get-goods-receipt-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.GetGoodsReceiptRawData](../../models/operations/get-goods-receipt-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |