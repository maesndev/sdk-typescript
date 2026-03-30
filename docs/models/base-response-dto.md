# BaseResponseDto

## Example Usage

```typescript
import { BaseResponseDto } from "@maesn/typescript-sdk/models";

let value: BaseResponseDto = {
  data: {},
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                   | Type                                    | Required                                | Description                             |
| --------------------------------------- | --------------------------------------- | --------------------------------------- | --------------------------------------- |
| `meta`                                  | [models.Meta](../models/meta.md)        | :heavy_minus_sign:                      | N/A                                     |
| `data`                                  | [models.Data](../models/data.md)        | :heavy_check_mark:                      | N/A                                     |
| `errors`                                | [models.Errors](../models/errors.md)    | :heavy_check_mark:                      | N/A                                     |
| `rawData`                               | [models.RawData](../models/raw-data.md) | :heavy_check_mark:                      | N/A                                     |