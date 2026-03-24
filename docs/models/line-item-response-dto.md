# LineItemResponseDto

## Example Usage

```typescript
import { LineItemResponseDto } from "maesn/models";

let value: LineItemResponseDto = {
  lineItemId: "<id>",
  accountId: "<id>",
  createdDate: {},
  description: "zowie best-seller aircraft misfire whoa inside",
  dimensions: [],
  discountItemAmount: 1897.07,
  discountItemPercentage: 4176.38,
  grossAmount: 6396.58,
  itemsAmount: 7645.06,
  itemId: "<id>",
  name: "<value>",
  quantity: 8198.95,
  taxCode: "<value>",
  taxRatePercentage: 9564.03,
  unitAmount: 2142.34,
  updatedDate: {},
};
```

## Fields

| Field                                                                                     | Type                                                                                      | Required                                                                                  | Description                                                                               |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `lineItemId`                                                                              | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `accountId`                                                                               | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `createdDate`                                                                             | [models.LineItemResponseDtoCreatedDate](../models/line-item-response-dto-created-date.md) | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `description`                                                                             | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `dimensions`                                                                              | [models.InvoiceDimensionResponseDto](../models/invoice-dimension-response-dto.md)[]       | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `discountItemAmount`                                                                      | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `discountItemPercentage`                                                                  | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `grossAmount`                                                                             | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `itemsAmount`                                                                             | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `itemId`                                                                                  | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `name`                                                                                    | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `quantity`                                                                                | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `taxCode`                                                                                 | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `taxRatePercentage`                                                                       | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `unitAmount`                                                                              | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `updatedDate`                                                                             | [models.LineItemResponseDtoUpdatedDate](../models/line-item-response-dto-updated-date.md) | :heavy_check_mark:                                                                        | N/A                                                                                       |