# BookingProposalLineItemResponseDtoV2

## Example Usage

```typescript
import { BookingProposalLineItemResponseDtoV2 } from "@maesn/typescript-sdk/models";

let value: BookingProposalLineItemResponseDtoV2 = {
  id: "<id>",
  account: {
    id: "<id>",
    code: "<value>",
    name: "<value>",
    number: 1700.36,
  },
  createdDate: "<value>",
  description: "nor until everlasting lobster",
  dimensions: [
    {
      id: "<id>",
      code: "<value>",
      dimension: "<value>",
      name: "<value>",
    },
  ],
  discountAmount: 3661.2,
  discountAmount2: 807.6,
  discountPercentage: 3281.69,
  discountPercentage2: 3275.46,
  taxCode: "<value>",
  taxRatePercentage: 6680.86,
  totalGrossAmount: 2827.73,
  totalNetAmount: 1757.47,
  type: "SERVICE",
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                                           | Type                                                                                                            | Required                                                                                                        | Description                                                                                                     |
| --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                            | *string*                                                                                                        | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
| `account`                                                                                                       | [models.Account](../models/account.md)                                                                          | :heavy_check_mark:                                                                                              | N/A                                                                                                             |
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