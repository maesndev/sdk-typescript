# GetUnitsResponse

List of units for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetUnitsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetUnitsResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `meta`                                                                      | [operations.GetUnitsMeta](../../models/operations/get-units-meta.md)        | :heavy_minus_sign:                                                          | N/A                                                                         |
| `data`                                                                      | [models.UnitResponseDto](../../models/unit-response-dto.md)[]               | :heavy_check_mark:                                                          | N/A                                                                         |
| `errors`                                                                    | [operations.GetUnitsErrors](../../models/operations/get-units-errors.md)    | :heavy_check_mark:                                                          | N/A                                                                         |
| `rawData`                                                                   | [operations.GetUnitsRawData](../../models/operations/get-units-raw-data.md) | :heavy_check_mark:                                                          | N/A                                                                         |