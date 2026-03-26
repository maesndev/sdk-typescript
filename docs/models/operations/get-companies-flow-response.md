# GetCompaniesFlowResponse

## Example Usage

```typescript
import { GetCompaniesFlowResponse } from "maesn/models/operations";

let value: GetCompaniesFlowResponse = {
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

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `meta`                                                                                       | [models.MetaResponse](../../models/meta-response.md)                                         | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.CompanyResponseDto](../../models/company-response-dto.md)[]                          | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.GetCompaniesFlowErrors](../../models/operations/get-companies-flow-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.GetCompaniesFlowRawData](../../models/operations/get-companies-flow-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |