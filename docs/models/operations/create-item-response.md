# CreateItemResponse

## Example Usage

```typescript
import { CreateItemResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateItemResponse = {
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
  rawData: null,
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `meta`                                                                          | [operations.CreateItemMeta](../../models/operations/create-item-meta.md)        | :heavy_minus_sign:                                                              | N/A                                                                             |
| `data`                                                                          | [models.ItemResponseDto](../../models/item-response-dto.md)                     | :heavy_check_mark:                                                              | N/A                                                                             |
| `errors`                                                                        | [operations.CreateItemErrors](../../models/operations/create-item-errors.md)    | :heavy_check_mark:                                                              | N/A                                                                             |
| `rawData`                                                                       | [operations.CreateItemRawData](../../models/operations/create-item-raw-data.md) | :heavy_check_mark:                                                              | N/A                                                                             |