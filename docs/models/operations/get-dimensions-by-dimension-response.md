# GetDimensionsByDimensionResponse

## Example Usage

```typescript
import { GetDimensionsByDimensionResponse } from "maesn/models/operations";

let value: GetDimensionsByDimensionResponse = {
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
      description: "excitedly unless knottily likewise absolve",
      dimension: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                         | Type                                                                                                          | Required                                                                                                      | Description                                                                                                   |
| ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                        | [models.MetaResponse](../../models/meta-response.md)                                                          | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `data`                                                                                                        | [models.DimensionMetaResponseDto](../../models/dimension-meta-response-dto.md)[]                              | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `errors`                                                                                                      | [operations.GetDimensionsByDimensionErrors](../../models/operations/get-dimensions-by-dimension-errors.md)    | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `rawData`                                                                                                     | [operations.GetDimensionsByDimensionRawData](../../models/operations/get-dimensions-by-dimension-raw-data.md) | :heavy_check_mark:                                                                                            | N/A                                                                                                           |