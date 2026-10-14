# GetReasonCodesResponse

List of reason codes for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetReasonCodesResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetReasonCodesResponse = {
  data: [],
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `meta`                                                                                   | [operations.GetReasonCodesMeta](../../models/operations/get-reason-codes-meta.md)        | :heavy_minus_sign:                                                                       | N/A                                                                                      |
| `data`                                                                                   | [models.ReasonCodeResponseDto](../../models/reason-code-response-dto.md)[]               | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `errors`                                                                                 | [operations.GetReasonCodesErrors](../../models/operations/get-reason-codes-errors.md)    | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `rawData`                                                                                | [operations.GetReasonCodesRawData](../../models/operations/get-reason-codes-raw-data.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |