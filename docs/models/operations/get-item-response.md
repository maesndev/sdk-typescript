# GetItemResponse

Item record matching the provided ID

## Example Usage

```typescript
import { GetItemResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetItemResponse = {
  data: [
    {
      id: "<id>",
      assetAccountId: "<id>",
      expenseAccountId: "<id>",
      incomeAccountId: null,
      inventoryStartDate: null,
      itemNumber: "<value>",
      lastModifiedDate: "<value>",
      name: "<value>",
      priceIncludesTax: null,
      stockCount: 1775.61,
      taxCode: "<value>",
      taxRatePercentage: 788.94,
      type: "PRODUCT",
      unitName: "STÜCK",
      unitPurchasePrice: 8202.63,
      unitSalesPrice: 8473.13,
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                     | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `meta`                                                                    | [operations.GetItemMeta](../../models/operations/get-item-meta.md)        | :heavy_minus_sign:                                                        | N/A                                                                       |
| `data`                                                                    | [models.ItemResponseDto](../../models/item-response-dto.md)[]             | :heavy_check_mark:                                                        | N/A                                                                       |
| `errors`                                                                  | [operations.GetItemErrors](../../models/operations/get-item-errors.md)    | :heavy_check_mark:                                                        | N/A                                                                       |
| `rawData`                                                                 | [operations.GetItemRawData](../../models/operations/get-item-raw-data.md) | :heavy_check_mark:                                                        | N/A                                                                       |