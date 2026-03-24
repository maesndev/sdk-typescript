# GetItemResponse

## Example Usage

```typescript
import { GetItemResponse } from "maesn/models/operations";

let value: GetItemResponse = {
  meta: {
    warnings: [
      "<value 1>",
      "<value 2>",
    ],
    pagination: {
      total: 3438.77,
      perPage: 5109.63,
      currentPage: 2626.79,
      totalPages: 3561.84,
    },
  },
  data: [
    {
      id: "<id>",
      assetAccountId: "<id>",
      expenseAccountId: "<id>",
      incomeAccountId: "<id>",
      inventoryStartDate: "<value>",
      itemNumber: "<value>",
      lastModifiedDate: "<value>",
      name: "<value>",
      priceIncludesTax: true,
      stockCount: 1233.95,
      taxCode: "<value>",
      taxRatePercentage: 1564.24,
      type: "PRODUCT",
      unitName: "STÜCK",
      unitPurchasePrice: 3317.13,
      unitSalesPrice: 4486.49,
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                     | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `meta`                                                                    | [models.MetaResponse](../../models/meta-response.md)                      | :heavy_check_mark:                                                        | N/A                                                                       |
| `data`                                                                    | [models.ItemResponseDto](../../models/item-response-dto.md)[]             | :heavy_check_mark:                                                        | N/A                                                                       |
| `errors`                                                                  | [operations.GetItemErrors](../../models/operations/get-item-errors.md)    | :heavy_check_mark:                                                        | N/A                                                                       |
| `rawData`                                                                 | [operations.GetItemRawData](../../models/operations/get-item-raw-data.md) | :heavy_check_mark:                                                        | N/A                                                                       |