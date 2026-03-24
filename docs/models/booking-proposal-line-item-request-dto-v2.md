# BookingProposalLineItemRequestDtoV2

## Example Usage

```typescript
import { BookingProposalLineItemRequestDtoV2 } from "maesn/models";

let value: BookingProposalLineItemRequestDtoV2 = {
  id: "<id>",
  account: {
    id: "<id>",
    code: "<value>",
    name: "<value>",
    number: 6545.39,
  },
  description: "even penalise warmhearted sweet",
  dimensions: [],
  discountAmount: 3647.17,
  discountAmount2: 9845.46,
  discountPercentage: 4894.01,
  discountPercentage2: 8308.2,
  taxCode: "<value>",
  taxRatePercentage: 328.07,
  totalGrossAmount: 212.6,
  totalNetAmount: 4237.01,
  type: "SERVICE",
};
```

## Fields

| Field                                                                                                         | Type                                                                                                          | Required                                                                                                      | Description                                                                                                   |
| ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| `id`                                                                                                          | *string*                                                                                                      | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `account`                                                                                                     | [models.AccountRequestCommonDtoV2](../models/account-request-common-dto-v2.md)                                | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `description`                                                                                                 | *string*                                                                                                      | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `dimensions`                                                                                                  | [models.DimensionRequestCommonDtoV2](../models/dimension-request-common-dto-v2.md)[]                          | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `discountAmount`                                                                                              | *number*                                                                                                      | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `discountAmount2`                                                                                             | *number*                                                                                                      | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `discountPercentage`                                                                                          | *number*                                                                                                      | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `discountPercentage2`                                                                                         | *number*                                                                                                      | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `taxCode`                                                                                                     | *string*                                                                                                      | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `taxRatePercentage`                                                                                           | *number*                                                                                                      | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `totalGrossAmount`                                                                                            | *number*                                                                                                      | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `totalNetAmount`                                                                                              | *number*                                                                                                      | :heavy_check_mark:                                                                                            | N/A                                                                                                           |
| `type`                                                                                                        | [models.BookingProposalLineItemRequestDtoV2Type](../models/booking-proposal-line-item-request-dto-v2-type.md) | :heavy_check_mark:                                                                                            | N/A                                                                                                           |