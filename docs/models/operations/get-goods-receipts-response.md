# GetGoodsReceiptsResponse

## Example Usage

```typescript
import { GetGoodsReceiptsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetGoodsReceiptsResponse = {
  data: [
    {
      id: "<id>",
      comment:
        "Boston's most advanced compression wear technology increases muscle oxygenation, stabilizes active muscles",
      createdDate: "<value>",
      description: "ugh seal toothbrush overwork sweetly",
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
    },
  ],
  errors: null,
  rawData: null,
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `meta`                                                                                       | [operations.GetGoodsReceiptsMeta](../../models/operations/get-goods-receipts-meta.md)        | :heavy_minus_sign:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.GoodsReceiptResponseDto](../../models/goods-receipt-response-dto.md)[]               | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.GetGoodsReceiptsErrors](../../models/operations/get-goods-receipts-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.GetGoodsReceiptsRawData](../../models/operations/get-goods-receipts-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |