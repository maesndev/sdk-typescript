# GetBillsResponse

## Example Usage

```typescript
import { GetBillsResponse } from "maesn/models/operations";

let value: GetBillsResponse = {
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

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `meta`                                                                      | [models.MetaResponse](../../models/meta-response.md)                        | :heavy_check_mark:                                                          | N/A                                                                         |
| `data`                                                                      | [models.BillResponseDto](../../models/bill-response-dto.md)[]               | :heavy_check_mark:                                                          | N/A                                                                         |
| `errors`                                                                    | [operations.GetBillsErrors](../../models/operations/get-bills-errors.md)    | :heavy_check_mark:                                                          | N/A                                                                         |
| `rawData`                                                                   | [operations.GetBillsRawData](../../models/operations/get-bills-raw-data.md) | :heavy_check_mark:                                                          | N/A                                                                         |