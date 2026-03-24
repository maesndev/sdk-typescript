# GetFiscalYearResponse

## Example Usage

```typescript
import { GetFiscalYearResponse } from "maesn/models/operations";

let value: GetFiscalYearResponse = {
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
  data: [
    {
      id: "<id>",
      accountNumberLength: 2914.24,
      chartOfAccount: "SKR04",
      createdDate: "<value>",
      description:
        "costume membership weep ugh verve inasmuch ah access repossess from",
      endDate: "<value>",
      startDate: "<value>",
      status: "OPEN",
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `meta`                                                                                 | [models.MetaResponse](../../models/meta-response.md)                                   | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `data`                                                                                 | [models.FiscalYearResponseDto](../../models/fiscal-year-response-dto.md)[]             | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `errors`                                                                               | [operations.GetFiscalYearErrors](../../models/operations/get-fiscal-year-errors.md)    | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `rawData`                                                                              | [operations.GetFiscalYearRawData](../../models/operations/get-fiscal-year-raw-data.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |