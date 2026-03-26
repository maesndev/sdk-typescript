# GetCompaniesResponse

## Example Usage

```typescript
import { GetCompaniesResponse } from "maesn/models/operations";

let value: GetCompaniesResponse = {
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

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `meta`                                                                              | [models.MetaResponse](../../models/meta-response.md)                                | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `data`                                                                              | [models.CompanyResponseDto](../../models/company-response-dto.md)[]                 | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `errors`                                                                            | [operations.GetCompaniesErrors](../../models/operations/get-companies-errors.md)    | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `rawData`                                                                           | [operations.GetCompaniesRawData](../../models/operations/get-companies-raw-data.md) | :heavy_check_mark:                                                                  | N/A                                                                                 |