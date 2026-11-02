# GetToleranceLimitsResponse

List of tolerance limits for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetToleranceLimitsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetToleranceLimitsResponse = {
  data: [],
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `meta`                                                                                           | [operations.GetToleranceLimitsMeta](../../models/operations/get-tolerance-limits-meta.md)        | :heavy_minus_sign:                                                                               | N/A                                                                                              |
| `data`                                                                                           | [models.ToleranceLimitResponseDto](../../models/tolerance-limit-response-dto.md)[]               | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `errors`                                                                                         | [operations.GetToleranceLimitsErrors](../../models/operations/get-tolerance-limits-errors.md)    | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `rawData`                                                                                        | [operations.GetToleranceLimitsRawData](../../models/operations/get-tolerance-limits-raw-data.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |