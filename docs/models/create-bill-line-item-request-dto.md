# CreateBillLineItemRequestDto

## Example Usage

```typescript
import { CreateBillLineItemRequestDto } from "maesn/models";

let value: CreateBillLineItemRequestDto = {
  id: "<id>",
  accountId: "<id>",
  accountNumber: "<value>",
  deferredEndDate: "<value>",
  deferredStartDate: "<value>",
  description: "fluff premier though boohoo nor",
  dimensions: [
    {
      name: "<value>",
      categoryName: "<value>",
    },
  ],
  itemId: "<id>",
  itemName: "<value>",
  quantity: 3963.74,
  taxCode: "<value>",
  taxRatePercentage: 2302.44,
  totalDiscountAmount: 2298.54,
  totalDiscountPercentage: 237.86,
  totalGrossAmount: 9929.17,
  totalNetAmount: 6725.62,
  totalTaxAmount: 6967.18,
  unitAmount: 2144.91,
  unitDiscountAmount: 8872.12,
  unitDiscountPercentage: 2184.99,
  unitName: "<value>",
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `id`                                                                        | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `accountId`                                                                 | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `accountNumber`                                                             | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `deferredEndDate`                                                           | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `deferredStartDate`                                                         | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `description`                                                               | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `dimensions`                                                                | [models.BillDimensionRequestDto](../models/bill-dimension-request-dto.md)[] | :heavy_check_mark:                                                          | N/A                                                                         |
| `itemId`                                                                    | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `itemName`                                                                  | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `quantity`                                                                  | *number*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `taxCode`                                                                   | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `taxRatePercentage`                                                         | *number*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `totalDiscountAmount`                                                       | *number*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `totalDiscountPercentage`                                                   | *number*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `totalGrossAmount`                                                          | *number*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `totalNetAmount`                                                            | *number*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `totalTaxAmount`                                                            | *number*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `unitAmount`                                                                | *number*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `unitDiscountAmount`                                                        | *number*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `unitDiscountPercentage`                                                    | *number*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `unitName`                                                                  | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |