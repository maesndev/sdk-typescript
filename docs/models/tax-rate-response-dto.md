# TaxRateResponseDto

## Example Usage

```typescript
import { TaxRateResponseDto } from "maesn/models";

let value: TaxRateResponseDto = {
  id: "<id>",
  code: "<value>",
  createdDate: {},
  description: "common by kick worth phooey along",
  name: "<value>",
  percentage: 4175.02,
  type: "NO_TAX",
  updatedDate: {},
  usage: "INVOICE",
};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `id`                                                                                    | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `code`                                                                                  | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `createdDate`                                                                           | [models.TaxRateResponseDtoCreatedDate](../models/tax-rate-response-dto-created-date.md) | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `description`                                                                           | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `name`                                                                                  | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `percentage`                                                                            | *number*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `type`                                                                                  | [models.TaxRateResponseDtoType](../models/tax-rate-response-dto-type.md)                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `updatedDate`                                                                           | [models.TaxRateResponseDtoUpdatedDate](../models/tax-rate-response-dto-updated-date.md) | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `usage`                                                                                 | [models.Usage](../models/usage.md)                                                      | :heavy_check_mark:                                                                      | N/A                                                                                     |