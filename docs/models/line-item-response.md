# LineItemResponse

## Example Usage

```typescript
import { LineItemResponse } from "@maesn/typescript-sdk/models";

let value: LineItemResponse = {
  id: null,
  accountCode: "<value>",
  accountId: "<id>",
  accountName: "<value>",
  accountNumber: 7712.93,
  bookingTaxCode: "<value>",
  createdDate: "<value>",
  description: "decent drat yet weatherize brr promise mmm march",
  dimension1: null,
  dimension2: "<value>",
  dimensions: [
    {
      id: "<id>",
      code: null,
      dimension: "<value>",
      name: "<value>",
    },
  ],
  discountAmount: 872.79,
  discountAmount2: 1511.36,
  discountPercentage: 2254.26,
  discountPercentage2: null,
  taxCode: "<value>",
  taxRatePercentage: 1405.29,
  totalGrossAmount: 7091.84,
  totalNetAmount: 7987.05,
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `id`                                                                                   | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `accountCode`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `accountId`                                                                            | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `accountName`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `accountNumber`                                                                        | *number*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `bookingTaxCode`                                                                       | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `createdDate`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `description`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `dimension1`                                                                           | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `dimension2`                                                                           | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `dimensions`                                                                           | [models.DimensionResponseCommonDtoV2](../models/dimension-response-common-dto-v2.md)[] | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `discountAmount`                                                                       | *number*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `discountAmount2`                                                                      | *number*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `discountPercentage`                                                                   | *number*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `discountPercentage2`                                                                  | *number*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `taxCode`                                                                              | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `taxRatePercentage`                                                                    | *number*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `totalGrossAmount`                                                                     | *number*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `totalNetAmount`                                                                       | *number*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `type`                                                                                 | [models.LineItemResponseType](../models/line-item-response-type.md)                    | :heavy_minus_sign:                                                                     | N/A                                                                                    |
| `updatedDate`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |