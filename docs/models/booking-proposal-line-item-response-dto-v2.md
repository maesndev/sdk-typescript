# BookingProposalLineItemResponseDtoV2

## Example Usage

```typescript
import { BookingProposalLineItemResponseDtoV2 } from "maesn/models";

let value: BookingProposalLineItemResponseDtoV2 = {
  id: "<id>",
  account: {
    id: "<id>",
    code: "<value>",
    name: "<value>",
    number: 6594.9,
  },
  createdDate: "<value>",
  description: "up minus certainly gee whoever",
  dimensions: [
    {
      id: "<id>",
      code: "<value>",
      dimension: "<value>",
      name: "<value>",
    },
  ],
  discountAmount: 5306.46,
  discountAmount2: 6308.36,
  discountPercentage: 5347.73,
  discountPercentage2: 3553.43,
  taxCode: "<value>",
  taxRatePercentage: 4343.78,
  totalGrossAmount: 5747.79,
  totalNetAmount: 6274.11,
  type: "PRODUCT",
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                                           | Type                                                                                                            | Required                                                                                                        | Description                                                                                                     |
| --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                            | *string*                                                                                                        | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `account`                                                                                                       | [models.AccountResponseCommonDtoV2](../models/account-response-common-dto-v2.md)                                | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `createdDate`                                                                                                   | *string*                                                                                                        | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `description`                                                                                                   | *string*                                                                                                        | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `dimensions`                                                                                                    | [models.DimensionResponseCommonDtoV2](../models/dimension-response-common-dto-v2.md)[]                          | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `discountAmount`                                                                                                | *number*                                                                                                        | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `discountAmount2`                                                                                               | *number*                                                                                                        | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `discountPercentage`                                                                                            | *number*                                                                                                        | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `discountPercentage2`                                                                                           | *number*                                                                                                        | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `taxCode`                                                                                                       | *string*                                                                                                        | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `taxRatePercentage`                                                                                             | *number*                                                                                                        | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `totalGrossAmount`                                                                                              | *number*                                                                                                        | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `totalNetAmount`                                                                                                | *number*                                                                                                        | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `type`                                                                                                          | [models.BookingProposalLineItemResponseDtoV2Type](../models/booking-proposal-line-item-response-dto-v2-type.md) | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `updatedDate`                                                                                                   | *string*                                                                                                        | :heavy_check_mark:                                                                                              | N/A                                                                                                             |