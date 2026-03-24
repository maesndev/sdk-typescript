# GetVendorCreditsResponse

## Example Usage

```typescript
import { GetVendorCreditsResponse } from "maesn/models/operations";

let value: GetVendorCreditsResponse = {
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
| `data`                                                                                       | [models.VendorCreditResponseDto](../../models/vendor-credit-response-dto.md)[]               | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.GetVendorCreditsErrors](../../models/operations/get-vendor-credits-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.GetVendorCreditsRawData](../../models/operations/get-vendor-credits-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |