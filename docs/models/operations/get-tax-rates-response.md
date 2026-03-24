# GetTaxRatesResponse

## Example Usage

```typescript
import { GetTaxRatesResponse } from "maesn/models/operations";

let value: GetTaxRatesResponse = {
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
      code: "<value>",
      createdDate: {},
      description: "or pessimistic gloom eek sharply",
      name: "<value>",
      percentage: 6598.68,
      type: "INCLUSIVE",
      updatedDate: {},
      usage: "BILL",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `meta`                                                                             | [models.MetaResponse](../../models/meta-response.md)                               | :heavy_check_mark:                                                                 | N/A                                                                                |
| `data`                                                                             | [models.TaxRateResponseDto](../../models/tax-rate-response-dto.md)[]               | :heavy_check_mark:                                                                 | N/A                                                                                |
| `errors`                                                                           | [operations.GetTaxRatesErrors](../../models/operations/get-tax-rates-errors.md)    | :heavy_check_mark:                                                                 | N/A                                                                                |
| `rawData`                                                                          | [operations.GetTaxRatesRawData](../../models/operations/get-tax-rates-raw-data.md) | :heavy_check_mark:                                                                 | N/A                                                                                |