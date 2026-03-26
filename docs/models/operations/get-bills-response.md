# GetBillsResponse

## Example Usage

```typescript
import { GetBillsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetBillsResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `meta`                                                                      | [operations.GetBillsMeta](../../models/operations/get-bills-meta.md)        | :heavy_minus_sign:                                                          | N/A                                                                         |
| `data`                                                                      | [models.BillResponseDto](../../models/bill-response-dto.md)[]               | :heavy_check_mark:                                                          | N/A                                                                         |
| `errors`                                                                    | [operations.GetBillsErrors](../../models/operations/get-bills-errors.md)    | :heavy_check_mark:                                                          | N/A                                                                         |
| `rawData`                                                                   | [operations.GetBillsRawData](../../models/operations/get-bills-raw-data.md) | :heavy_check_mark:                                                          | N/A                                                                         |