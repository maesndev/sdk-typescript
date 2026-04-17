# PatchLineItemResponse

Line item updated successfully

## Example Usage

```typescript
import { PatchLineItemResponse } from "@maesn/typescript-sdk/models/operations";

let value: PatchLineItemResponse = {
  data: {
    lineItemId: "<id>",
    accountId: "<id>",
    createdDate: "<value>",
    description: "out kindly unselfish",
    dimensions: [
      {
        id: "<id>",
        categoryName: "<value>",
        name: null,
      },
    ],
    discountItemAmount: 1433.15,
    discountItemPercentage: 9792.95,
    grossAmount: null,
    itemsAmount: 3815.51,
    itemId: "<id>",
    name: "<value>",
    quantity: 8444.65,
    taxRatePercentage: null,
    unitAmount: 7360.37,
    updatedDate: "<value>",
  },
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `meta`                                                                                 | [operations.PatchLineItemMeta](../../models/operations/patch-line-item-meta.md)        | :heavy_minus_sign:                                                                     | N/A                                                                                    |
| `data`                                                                                 | [models.LineItemResponseDto](../../models/line-item-response-dto.md)                   | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `errors`                                                                               | [operations.PatchLineItemErrors](../../models/operations/patch-line-item-errors.md)    | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `rawData`                                                                              | [operations.PatchLineItemRawData](../../models/operations/patch-line-item-raw-data.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |