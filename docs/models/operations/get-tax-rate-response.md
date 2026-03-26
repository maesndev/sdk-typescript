# GetTaxRateResponse

## Example Usage

```typescript
import { GetTaxRateResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetTaxRateResponse = {
  data: {
    id: "<id>",
    code: "<value>",
    createdDate: "<value>",
    description: "likewise ouch excluding astride worriedly nasalise ick far",
    name: "<value>",
    percentage: 5469.19,
    type: "ZERO_TAX",
    updatedDate: "<value>",
    usage: "ALL",
  },
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                            | Type                                                                             | Required                                                                         | Description                                                                      |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `meta`                                                                           | [operations.GetTaxRateMeta](../../models/operations/get-tax-rate-meta.md)        | :heavy_minus_sign:                                                               | N/A                                                                              |
| `data`                                                                           | [models.TaxRateResponseDto](../../models/tax-rate-response-dto.md)               | :heavy_check_mark:                                                               | N/A                                                                              |
| `errors`                                                                         | [operations.GetTaxRateErrors](../../models/operations/get-tax-rate-errors.md)    | :heavy_check_mark:                                                               | N/A                                                                              |
| `rawData`                                                                        | [operations.GetTaxRateRawData](../../models/operations/get-tax-rate-raw-data.md) | :heavy_check_mark:                                                               | N/A                                                                              |