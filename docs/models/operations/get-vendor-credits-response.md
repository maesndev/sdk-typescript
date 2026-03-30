# GetVendorCreditsResponse

List of vendor credits for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetVendorCreditsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetVendorCreditsResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `meta`                                                                                       | [operations.GetVendorCreditsMeta](../../models/operations/get-vendor-credits-meta.md)        | :heavy_minus_sign:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.VendorCreditResponseDto](../../models/vendor-credit-response-dto.md)[]               | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.GetVendorCreditsErrors](../../models/operations/get-vendor-credits-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.GetVendorCreditsRawData](../../models/operations/get-vendor-credits-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |