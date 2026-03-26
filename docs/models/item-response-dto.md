# ItemResponseDto

## Example Usage

```typescript
import { ItemResponseDto } from "@maesn/typescript-sdk/models";

let value: ItemResponseDto = {
  id: "<id>",
  assetAccountId: "<id>",
  expenseAccountId: "<id>",
  incomeAccountId: "<id>",
  inventoryStartDate: "<value>",
  itemNumber: "<value>",
  lastModifiedDate: "<value>",
  name: "<value>",
  priceIncludesTax: true,
  stockCount: null,
  taxCode: "<value>",
  taxRatePercentage: 9240.74,
  type: "SERVICE",
  unitName: "LITRE",
  unitPurchasePrice: 1226.15,
  unitSalesPrice: 7169.79,
};
```

## Fields

| Field                                                                      | Type                                                                       | Required                                                                   | Description                                                                |
| -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| `id`                                                                       | *string*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `assetAccountId`                                                           | *string*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `expenseAccountId`                                                         | *string*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `incomeAccountId`                                                          | *string*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `inventoryStartDate`                                                       | *string*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `itemNumber`                                                               | *string*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `lastModifiedDate`                                                         | *string*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `name`                                                                     | *string*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `priceIncludesTax`                                                         | *boolean*                                                                  | :heavy_check_mark:                                                         | N/A                                                                        |
| `stockCount`                                                               | *number*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `taxCode`                                                                  | *string*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `taxRatePercentage`                                                        | *number*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `type`                                                                     | [models.ItemResponseDtoType](../models/item-response-dto-type.md)          | :heavy_check_mark:                                                         | N/A                                                                        |
| `unitName`                                                                 | [models.ItemResponseDtoUnitName](../models/item-response-dto-unit-name.md) | :heavy_check_mark:                                                         | N/A                                                                        |
| `unitPurchasePrice`                                                        | *number*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `unitSalesPrice`                                                           | *number*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |