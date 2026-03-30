# GetFiscalYearsResponse

List of fiscal years for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetFiscalYearsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetFiscalYearsResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `meta`                                                                                   | [operations.GetFiscalYearsMeta](../../models/operations/get-fiscal-years-meta.md)        | :heavy_minus_sign:                                                                       | N/A                                                                                      |
| `data`                                                                                   | [models.FiscalYearResponseDto](../../models/fiscal-year-response-dto.md)[]               | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `errors`                                                                                 | [operations.GetFiscalYearsErrors](../../models/operations/get-fiscal-years-errors.md)    | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `rawData`                                                                                | [operations.GetFiscalYearsRawData](../../models/operations/get-fiscal-years-raw-data.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |