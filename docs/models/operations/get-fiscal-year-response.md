# GetFiscalYearResponse

## Example Usage

```typescript
import { GetFiscalYearResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetFiscalYearResponse = {
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
| `meta`                                                                                 | [operations.GetFiscalYearMeta](../../models/operations/get-fiscal-year-meta.md)        | :heavy_minus_sign:                                                                     | N/A                                                                                    |
| `data`                                                                                 | [models.FiscalYearResponseDto](../../models/fiscal-year-response-dto.md)[]             | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `errors`                                                                               | [operations.GetFiscalYearErrors](../../models/operations/get-fiscal-year-errors.md)    | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `rawData`                                                                              | [operations.GetFiscalYearRawData](../../models/operations/get-fiscal-year-raw-data.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |