# GetEnvironmentsResponse

List of environments for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetEnvironmentsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetEnvironmentsResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                     | Type                                                                                      | Required                                                                                  | Description                                                                               |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `meta`                                                                                    | [operations.GetEnvironmentsMeta](../../models/operations/get-environments-meta.md)        | :heavy_minus_sign:                                                                        | N/A                                                                                       |
| `data`                                                                                    | [models.EnvironmentResponseDto](../../models/environment-response-dto.md)[]               | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `errors`                                                                                  | [operations.GetEnvironmentsErrors](../../models/operations/get-environments-errors.md)    | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `rawData`                                                                                 | [operations.GetEnvironmentsRawData](../../models/operations/get-environments-raw-data.md) | :heavy_check_mark:                                                                        | N/A                                                                                       |