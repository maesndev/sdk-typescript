# BillLineItemResponseDto

## Example Usage

```typescript
import { BillLineItemResponseDto } from "@maesn/typescript-sdk/models";

let value: BillLineItemResponseDto = {
  id: "<id>",
  accountId: "<id>",
  accountNumber: "<value>",
  createdDate: "<value>",
  deferredEndDate: "<value>",
  deferredStartDate: "<value>",
  description: "fort bah during bah kick",
  dimensions: [
    {
      name: "<value>",
      categoryName: "<value>",
    },
  ],
  itemId: "<id>",
  itemName: "<value>",
  quantity: 257.98,
  taxCode: null,
  taxRatePercentage: 7510.8,
  totalDiscountAmount: 2735.39,
  totalDiscountPercentage: 3029.15,
  totalGrossAmount: 6234.4,
  totalNetAmount: 5665.36,
  totalTaxAmount: 6761.91,
  unitAmount: null,
  unitDiscountAmount: null,
  unitDiscountPercentage: 3035.99,
  unitName: "<value>",
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `id`                                                                          | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `accountId`                                                                   | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `accountNumber`                                                               | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `createdDate`                                                                 | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `deferredEndDate`                                                             | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `deferredStartDate`                                                           | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `description`                                                                 | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `dimensions`                                                                  | [models.BillDimensionResponseDto](../models/bill-dimension-response-dto.md)[] | :heavy_check_mark:                                                            | N/A                                                                           |
| `itemId`                                                                      | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `itemName`                                                                    | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `quantity`                                                                    | *number*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `taxCode`                                                                     | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `taxRatePercentage`                                                           | *number*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `totalDiscountAmount`                                                         | *number*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `totalDiscountPercentage`                                                     | *number*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `totalGrossAmount`                                                            | *number*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `totalNetAmount`                                                              | *number*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `totalTaxAmount`                                                              | *number*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `unitAmount`                                                                  | *number*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `unitDiscountAmount`                                                          | *number*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `unitDiscountPercentage`                                                      | *number*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `unitName`                                                                    | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `updatedDate`                                                                 | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |