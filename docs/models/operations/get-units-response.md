# GetUnitsResponse

## Example Usage

```typescript
import { GetUnitsResponse } from "maesn/models/operations";

let value: GetUnitsResponse = {
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
| `data`                                                                      | [models.UnitResponseDto](../../models/unit-response-dto.md)[]               | :heavy_check_mark:                                                          | N/A                                                                         |
| `errors`                                                                    | [operations.GetUnitsErrors](../../models/operations/get-units-errors.md)    | :heavy_check_mark:                                                          | N/A                                                                         |
| `rawData`                                                                   | [operations.GetUnitsRawData](../../models/operations/get-units-raw-data.md) | :heavy_check_mark:                                                          | N/A                                                                         |