# GetDimensionsResponse

## Example Usage

```typescript
import { GetDimensionsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetDimensionsResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [operations.GetDimensionsMeta](../../models/operations/get-dimensions-meta.md)        | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `data`                                                                                | [models.DimensionResponseDto](../../models/dimension-response-dto.md)[]               | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.GetDimensionsErrors](../../models/operations/get-dimensions-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.GetDimensionsRawData](../../models/operations/get-dimensions-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |