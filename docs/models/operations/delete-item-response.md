# DeleteItemResponse

Item deleted successfully

## Example Usage

```typescript
import { DeleteItemResponse } from "@maesn/typescript-sdk/models/operations";

let value: DeleteItemResponse = {
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
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `meta`                                                                          | [operations.DeleteItemMeta](../../models/operations/delete-item-meta.md)        | :heavy_minus_sign:                                                              | N/A                                                                             |
| `data`                                                                          | [models.ItemResponseDto](../../models/item-response-dto.md)                     | :heavy_check_mark:                                                              | N/A                                                                             |
| `errors`                                                                        | [operations.DeleteItemErrors](../../models/operations/delete-item-errors.md)    | :heavy_check_mark:                                                              | N/A                                                                             |
| `rawData`                                                                       | [operations.DeleteItemRawData](../../models/operations/delete-item-raw-data.md) | :heavy_check_mark:                                                              | N/A                                                                             |