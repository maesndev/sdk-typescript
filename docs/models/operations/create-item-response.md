# CreateItemResponse

## Example Usage

```typescript
import { CreateItemResponse } from "maesn/models/operations";

let value: CreateItemResponse = {
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

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `meta`                                                                          | [models.MetaResponse](../../models/meta-response.md)                            | :heavy_check_mark:                                                              | N/A                                                                             |
| `data`                                                                          | [models.ItemResponseDto](../../models/item-response-dto.md)[]                   | :heavy_check_mark:                                                              | N/A                                                                             |
| `errors`                                                                        | [operations.CreateItemErrors](../../models/operations/create-item-errors.md)    | :heavy_check_mark:                                                              | N/A                                                                             |
| `rawData`                                                                       | [operations.CreateItemRawData](../../models/operations/create-item-raw-data.md) | :heavy_check_mark:                                                              | N/A                                                                             |