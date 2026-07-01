# GetDimensionsByDimensionV2Response

List of dimension values for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetDimensionsByDimensionV2Response } from "@maesn/typescript-sdk/models/operations";

let value: GetDimensionsByDimensionV2Response = {
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

| Field                                                                                                              | Type                                                                                                               | Required                                                                                                           | Description                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `meta`                                                                                                             | [operations.GetDimensionsByDimensionV2Meta](../../models/operations/get-dimensions-by-dimension-v2-meta.md)        | :heavy_minus_sign:                                                                                                 | N/A                                                                                                                |
| `data`                                                                                                             | [models.DimensionMetaResponseDto](../../models/dimension-meta-response-dto.md)[]                                   | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `errors`                                                                                                           | [operations.GetDimensionsByDimensionV2Errors](../../models/operations/get-dimensions-by-dimension-v2-errors.md)    | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |
| `rawData`                                                                                                          | [operations.GetDimensionsByDimensionV2RawData](../../models/operations/get-dimensions-by-dimension-v2-raw-data.md) | :heavy_check_mark:                                                                                                 | N/A                                                                                                                |