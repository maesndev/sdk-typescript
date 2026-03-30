# GetCompaniesFlowResponse

List of companies for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetCompaniesFlowResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetCompaniesFlowResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `meta`                                                                                       | [operations.GetCompaniesFlowMeta](../../models/operations/get-companies-flow-meta.md)        | :heavy_minus_sign:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.CompanyResponseDto](../../models/company-response-dto.md)[]                          | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.GetCompaniesFlowErrors](../../models/operations/get-companies-flow-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.GetCompaniesFlowRawData](../../models/operations/get-companies-flow-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |