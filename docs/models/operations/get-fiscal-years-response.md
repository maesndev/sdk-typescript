# GetFiscalYearsResponse

## Example Usage

```typescript
import { GetFiscalYearsResponse } from "maesn/models/operations";

let value: GetFiscalYearsResponse = {
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
| `data`                                                                                   | [models.FiscalYearResponseDto](../../models/fiscal-year-response-dto.md)[]               | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `errors`                                                                                 | [operations.GetFiscalYearsErrors](../../models/operations/get-fiscal-years-errors.md)    | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `rawData`                                                                                | [operations.GetFiscalYearsRawData](../../models/operations/get-fiscal-years-raw-data.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |