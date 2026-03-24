# PatchItemRequestDto

## Example Usage

```typescript
import { PatchItemRequestDto } from "maesn/models";

let value: PatchItemRequestDto = {
  name: "<value>",
  itemNumber: "<value>",
  stockCount: 8229.39,
  type: "SERVICE",
  unitName: "MILLIGRAM",
  unitPurchasePrice: 7627.04,
  unitSalesPrice: 6633.84,
  priceIncludesTax: true,
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `name`                                                                              | *string*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `itemNumber`                                                                        | *string*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `stockCount`                                                                        | *number*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `type`                                                                              | [models.PatchItemRequestDtoType](../models/patch-item-request-dto-type.md)          | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `unitName`                                                                          | [models.PatchItemRequestDtoUnitName](../models/patch-item-request-dto-unit-name.md) | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `unitPurchasePrice`                                                                 | *number*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `unitSalesPrice`                                                                    | *number*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `priceIncludesTax`                                                                  | *boolean*                                                                           | :heavy_check_mark:                                                                  | N/A                                                                                 |