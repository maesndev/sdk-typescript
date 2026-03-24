# CreateItemRequestDto

## Example Usage

```typescript
import { CreateItemRequestDto } from "maesn/models";

let value: CreateItemRequestDto = {
  assetAccountId: "<id>",
  expenseAccountId: "<id>",
  incomeAccountId: "<id>",
  inventoryStartDate: "<value>",
  itemNumber: "<value>",
  name: "<value>",
  priceIncludesTax: false,
  stockCount: 8861.3,
  taxCode: "<value>",
  taxRatePercentage: 3642.2,
  type: "PRODUCT",
  unitName: "CUBIC_METRE",
  unitPurchasePrice: 951.93,
  unitSalesPrice: 1401.96,
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `assetAccountId`                                                                      | *string*                                                                              | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `expenseAccountId`                                                                    | *string*                                                                              | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `incomeAccountId`                                                                     | *string*                                                                              | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `inventoryStartDate`                                                                  | *string*                                                                              | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `itemNumber`                                                                          | *string*                                                                              | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `name`                                                                                | *string*                                                                              | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `priceIncludesTax`                                                                    | *boolean*                                                                             | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `stockCount`                                                                          | *number*                                                                              | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `taxCode`                                                                             | *string*                                                                              | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `taxRatePercentage`                                                                   | *number*                                                                              | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `type`                                                                                | [models.CreateItemRequestDtoType](../models/create-item-request-dto-type.md)          | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `unitName`                                                                            | [models.CreateItemRequestDtoUnitName](../models/create-item-request-dto-unit-name.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `unitPurchasePrice`                                                                   | *number*                                                                              | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `unitSalesPrice`                                                                      | *number*                                                                              | :heavy_check_mark:                                                                    | N/A                                                                                   |