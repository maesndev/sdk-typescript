# GetGoodsReceiptsResponse

## Example Usage

```typescript
import { GetGoodsReceiptsResponse } from "maesn/models/operations";

let value: GetGoodsReceiptsResponse = {
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
      comment:
        "The Apollotech B340 is an affordable wireless mouse with reliable connectivity, 12 months battery life and modern design",
      createdDate: "<value>",
      description: "oof phooey sheepishly after criminal coin",
      lineItems: [],
      reference: "<value>",
      supplierId: "<id>",
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `meta`                                                                                       | [models.MetaResponse](../../models/meta-response.md)                                         | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.GoodsReceiptResponseDto](../../models/goods-receipt-response-dto.md)[]               | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.GetGoodsReceiptsErrors](../../models/operations/get-goods-receipts-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.GetGoodsReceiptsRawData](../../models/operations/get-goods-receipts-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |