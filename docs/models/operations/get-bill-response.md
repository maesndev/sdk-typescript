# GetBillResponse

## Example Usage

```typescript
import { GetBillResponse } from "maesn/models/operations";

let value: GetBillResponse = {
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

| Field                                                                     | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `meta`                                                                    | [models.MetaResponse](../../models/meta-response.md)                      | :heavy_check_mark:                                                        | N/A                                                                       |
| `data`                                                                    | [models.BillResponseDto](../../models/bill-response-dto.md)[]             | :heavy_check_mark:                                                        | N/A                                                                       |
| `errors`                                                                  | [operations.GetBillErrors](../../models/operations/get-bill-errors.md)    | :heavy_check_mark:                                                        | N/A                                                                       |
| `rawData`                                                                 | [operations.GetBillRawData](../../models/operations/get-bill-raw-data.md) | :heavy_check_mark:                                                        | N/A                                                                       |