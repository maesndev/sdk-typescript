# GetTaxRateResponse

## Example Usage

```typescript
import { GetTaxRateResponse } from "maesn/models/operations";

let value: GetTaxRateResponse = {
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
  data: {
    id: "<id>",
    code: "<value>",
    createdDate: {},
    description: "primary to or provided yuck pale male",
    name: "<value>",
    percentage: 292,
    type: "ZERO_TAX",
    updatedDate: {},
    usage: "ALL",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                            | Type                                                                             | Required                                                                         | Description                                                                      |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `meta`                                                                           | [models.MetaResponse](../../models/meta-response.md)                             | :heavy_check_mark:                                                               | N/A                                                                              |
| `data`                                                                           | [models.TaxRateResponseDto](../../models/tax-rate-response-dto.md)               | :heavy_check_mark:                                                               | N/A                                                                              |
| `errors`                                                                         | [operations.GetTaxRateErrors](../../models/operations/get-tax-rate-errors.md)    | :heavy_check_mark:                                                               | N/A                                                                              |
| `rawData`                                                                        | [operations.GetTaxRateRawData](../../models/operations/get-tax-rate-raw-data.md) | :heavy_check_mark:                                                               | N/A                                                                              |