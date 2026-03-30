# GetGoodsReceiptLineItemsResponse

List of line items for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetGoodsReceiptLineItemsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetGoodsReceiptLineItemsResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                          | Type                                                                                                           | Required                                                                                                       | Description                                                                                                    |
| -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                         | [operations.GetGoodsReceiptLineItemsMeta](../../models/operations/get-goods-receipt-line-items-meta.md)        | :heavy_minus_sign:                                                                                             | N/A                                                                                                            |
| `data`                                                                                                         | [models.GoodsReceiptLineItemResponse](../../models/goods-receipt-line-item-response.md)[]                      | :heavy_check_mark:                                                                                             | N/A                                                                                                            |
| `errors`                                                                                                       | [operations.GetGoodsReceiptLineItemsErrors](../../models/operations/get-goods-receipt-line-items-errors.md)    | :heavy_check_mark:                                                                                             | N/A                                                                                                            |
| `rawData`                                                                                                      | [operations.GetGoodsReceiptLineItemsRawData](../../models/operations/get-goods-receipt-line-items-raw-data.md) | :heavy_check_mark:                                                                                             | N/A                                                                                                            |