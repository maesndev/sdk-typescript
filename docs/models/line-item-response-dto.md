# LineItemResponseDto

## Example Usage

```typescript
import { LineItemResponseDto } from "@maesn/typescript-sdk/models";

let value: LineItemResponseDto = {
  lineItemId: "<id>",
  accountId: "<id>",
  createdDate: "<value>",
  description: "finally outset clone",
  dimensions: [],
  discountItemAmount: 524.18,
  discountItemPercentage: 5350.14,
  grossAmount: null,
  itemsAmount: 8917.02,
  itemId: "<id>",
  name: "<value>",
  quantity: 9174.54,
  taxRatePercentage: null,
  unitAmount: 8890.53,
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `lineItemId`                                                                        | *string*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `accountId`                                                                         | *string*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `createdDate`                                                                       | *string*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `description`                                                                       | *string*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `dimensions`                                                                        | [models.InvoiceDimensionResponseDto](../models/invoice-dimension-response-dto.md)[] | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `discountItemAmount`                                                                | *number*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `discountItemPercentage`                                                            | *number*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `grossAmount`                                                                       | *number*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `itemsAmount`                                                                       | *number*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `itemId`                                                                            | *string*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `name`                                                                              | *string*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `quantity`                                                                          | *number*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `taxCode`                                                                           | *string*                                                                            | :heavy_minus_sign:                                                                  | N/A                                                                                 |
| `taxRatePercentage`                                                                 | *number*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `unitAmount`                                                                        | *number*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `updatedDate`                                                                       | *string*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |