# GetDimensionsByDimensionResponse

## Example Usage

```typescript
import { GetDimensionsByDimensionResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetDimensionsByDimensionResponse = {
  data: [
    {
      description: "loftily although tomorrow until hm summarise",
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
| `meta`                                                                                                        | [operations.GetDimensionsByDimensionMeta](../../models/operations/get-dimensions-by-dimension-meta.md)        | :heavy_minus_sign:                                                                                            | N/A                                                                                                           |
| `data`                                                                                                        | [models.DimensionMetaResponseDto](../../models/dimension-meta-response-dto.md)[]                              | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `errors`                                                                                                      | [operations.GetDimensionsByDimensionErrors](../../models/operations/get-dimensions-by-dimension-errors.md)    | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `rawData`                                                                                                     | [operations.GetDimensionsByDimensionRawData](../../models/operations/get-dimensions-by-dimension-raw-data.md) | :heavy_check_mark:                                                                                            | N/A                                                                                                           |