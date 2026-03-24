# CreateLineItemResponse

## Example Usage

```typescript
import { CreateLineItemResponse } from "maesn/models/operations";

let value: CreateLineItemResponse = {
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

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `meta`                                                                                   | [models.MetaResponse](../../models/meta-response.md)                                     | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `data`                                                                                   | [models.LineItemResponseDto](../../models/line-item-response-dto.md)[]                   | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `errors`                                                                                 | [operations.CreateLineItemErrors](../../models/operations/create-line-item-errors.md)    | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `rawData`                                                                                | [operations.CreateLineItemRawData](../../models/operations/create-line-item-raw-data.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |