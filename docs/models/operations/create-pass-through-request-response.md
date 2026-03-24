# CreatePassThroughRequestResponse

## Example Usage

```typescript
import { CreatePassThroughRequestResponse } from "maesn/models/operations";

let value: CreatePassThroughRequestResponse = {
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
  data: {},
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                         | Type                                                                                                          | Required                                                                                                      | Description                                                                                                   |
| ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                        | [models.MetaResponse](../../models/meta-response.md)                                                          | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `data`                                                                                                        | [operations.Data](../../models/operations/data.md)                                                            | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `errors`                                                                                                      | [operations.CreatePassThroughRequestErrors](../../models/operations/create-pass-through-request-errors.md)    | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `rawData`                                                                                                     | [operations.CreatePassThroughRequestRawData](../../models/operations/create-pass-through-request-raw-data.md) | :heavy_check_mark:                                                                                            | N/A                                                                                                           |