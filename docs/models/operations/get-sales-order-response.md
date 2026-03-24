# GetSalesOrderResponse

## Example Usage

```typescript
import { GetSalesOrderResponse } from "maesn/models/operations";

let value: GetSalesOrderResponse = {
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

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `meta`                                                                                 | [models.MetaResponse](../../models/meta-response.md)                                   | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `data`                                                                                 | [models.SalesOrderResponseDto](../../models/sales-order-response-dto.md)[]             | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `errors`                                                                               | [operations.GetSalesOrderErrors](../../models/operations/get-sales-order-errors.md)    | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `rawData`                                                                              | [operations.GetSalesOrderRawData](../../models/operations/get-sales-order-raw-data.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |