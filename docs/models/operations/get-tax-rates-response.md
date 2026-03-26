# GetTaxRatesResponse

## Example Usage

```typescript
import { GetTaxRatesResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetTaxRatesResponse = {
  data: [
    {
      id: "<id>",
      code: "<value>",
      createdDate: "<value>",
      description: "through pastel before vary loftily",
      name: "<value>",
      percentage: 2766.58,
      type: "NO_TAX",
      updatedDate: "<value>",
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
| `meta`                                                                             | [operations.GetTaxRatesMeta](../../models/operations/get-tax-rates-meta.md)        | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `data`                                                                             | [models.TaxRateResponseDto](../../models/tax-rate-response-dto.md)[]               | :heavy_check_mark:                                                                 | N/A                                                                                |
| `errors`                                                                           | [operations.GetTaxRatesErrors](../../models/operations/get-tax-rates-errors.md)    | :heavy_check_mark:                                                                 | N/A                                                                                |
| `rawData`                                                                          | [operations.GetTaxRatesRawData](../../models/operations/get-tax-rates-raw-data.md) | :heavy_check_mark:                                                                 | N/A                                                                                |