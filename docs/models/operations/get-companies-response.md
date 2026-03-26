# GetCompaniesResponse

## Example Usage

```typescript
import { GetCompaniesResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetCompaniesResponse = {
  data: [],
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `meta`                                                                              | [operations.GetCompaniesMeta](../../models/operations/get-companies-meta.md)        | :heavy_minus_sign:                                                                  | N/A                                                                                 |
| `data`                                                                              | [models.CompanyResponseDto](../../models/company-response-dto.md)[]                 | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `errors`                                                                            | [operations.GetCompaniesErrors](../../models/operations/get-companies-errors.md)    | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `rawData`                                                                           | [operations.GetCompaniesRawData](../../models/operations/get-companies-raw-data.md) | :heavy_check_mark:                                                                  | N/A                                                                                 |