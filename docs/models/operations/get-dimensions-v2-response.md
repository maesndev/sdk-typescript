# GetDimensionsV2Response

## Example Usage

```typescript
import { GetDimensionsV2Response } from "@maesn/typescript-sdk/models/operations";

let value: GetDimensionsV2Response = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `meta`                                                                                     | [operations.GetDimensionsV2Meta](../../models/operations/get-dimensions-v2-meta.md)        | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.DimensionMetaResponseDto](../../models/dimension-meta-response-dto.md)[]           | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.GetDimensionsV2Errors](../../models/operations/get-dimensions-v2-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.GetDimensionsV2RawData](../../models/operations/get-dimensions-v2-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |