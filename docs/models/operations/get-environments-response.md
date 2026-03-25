# GetEnvironmentsResponse

## Example Usage

```typescript
import { GetEnvironmentsResponse } from "maesn/models/operations";

let value: GetEnvironmentsResponse = {
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

| Field                                                                                     | Type                                                                                      | Required                                                                                  | Description                                                                               |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `meta`                                                                                    | [models.MetaResponse](../../models/meta-response.md)                                      | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `data`                                                                                    | [models.EnvironmentResponseDto](../../models/environment-response-dto.md)[]               | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `errors`                                                                                  | [operations.GetEnvironmentsErrors](../../models/operations/get-environments-errors.md)    | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `rawData`                                                                                 | [operations.GetEnvironmentsRawData](../../models/operations/get-environments-raw-data.md) | :heavy_check_mark:                                                                        | N/A                                                                                       |