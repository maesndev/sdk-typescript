# PatchItemResponse

Item updated successfully

## Example Usage

```typescript
import { PatchItemResponse } from "@maesn/typescript-sdk/models/operations";

let value: PatchItemResponse = {
  data: {
    id: "<id>",
    assetAccountId: "<id>",
    expenseAccountId: "<id>",
    incomeAccountId: "<id>",
    inventoryStartDate: "<value>",
    itemNumber: "<value>",
    lastModifiedDate: "<value>",
    name: "<value>",
    priceIncludesTax: false,
    stockCount: 4368.68,
    taxCode: "<value>",
    taxRatePercentage: null,
    type: "PRODUCT",
    unitName: "PIECE",
    unitPurchasePrice: 1170.1,
    unitSalesPrice: null,
  },
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `meta`                                                                        | [operations.PatchItemMeta](../../models/operations/patch-item-meta.md)        | :heavy_minus_sign:                                                            | N/A                                                                           |
| `data`                                                                        | [models.ItemResponseDto](../../models/item-response-dto.md)                   | :heavy_check_mark:                                                            | N/A                                                                           |
| `errors`                                                                      | [operations.PatchItemErrors](../../models/operations/patch-item-errors.md)    | :heavy_check_mark:                                                            | N/A                                                                           |
| `rawData`                                                                     | [operations.PatchItemRawData](../../models/operations/patch-item-raw-data.md) | :heavy_check_mark:                                                            | N/A                                                                           |