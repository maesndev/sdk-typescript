# TaxRateResponseDto

## Example Usage

```typescript
import { TaxRateResponseDto } from "@maesn/typescript-sdk/models";

let value: TaxRateResponseDto = {
  id: "<id>",
  code: "<value>",
  createdDate: "<value>",
  description: "limply antagonize woot condense who yippee",
  name: "<value>",
  percentage: 707.74,
  type: "NO_TAX",
  updatedDate: "<value>",
  usage: "INVOICE",
};
```

## Fields

| Field                                                                    | Type                                                                     | Required                                                                 | Description                                                              |
| ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ |
| `id`                                                                     | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `code`                                                                   | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `createdDate`                                                            | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `description`                                                            | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `name`                                                                   | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `percentage`                                                             | *number*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `type`                                                                   | [models.TaxRateResponseDtoType](../models/tax-rate-response-dto-type.md) | :heavy_check_mark:                                                       | N/A                                                                      |
| `updatedDate`                                                            | *string*                                                                 | :heavy_check_mark:                                                       | N/A                                                                      |
| `usage`                                                                  | [models.Usage](../models/usage.md)                                       | :heavy_check_mark:                                                       | N/A                                                                      |