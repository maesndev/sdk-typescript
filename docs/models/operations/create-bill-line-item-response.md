# CreateBillLineItemResponse

## Example Usage

```typescript
import { CreateBillLineItemResponse } from "maesn/models/operations";

let value: CreateBillLineItemResponse = {
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

| Field                                                                                             | Type                                                                                              | Required                                                                                          | Description                                                                                       |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `meta`                                                                                            | [models.MetaResponse](../../models/meta-response.md)                                              | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `data`                                                                                            | [models.BillLineItemResponseDto](../../models/bill-line-item-response-dto.md)[]                   | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `errors`                                                                                          | [operations.CreateBillLineItemErrors](../../models/operations/create-bill-line-item-errors.md)    | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `rawData`                                                                                         | [operations.CreateBillLineItemRawData](../../models/operations/create-bill-line-item-raw-data.md) | :heavy_check_mark:                                                                                | N/A                                                                                               |