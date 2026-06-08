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
        name: "<value>",
      },
    ],
    discountItemAmount: 784.75,
    discountItemPercentage: 3815.51,
    grossAmount: 7430.87,
    itemsAmount: 8444.65,
    itemId: null,
    name: "<value>",
    quantity: 3749.43,
    taxCode: "<value>",
    taxRatePercentage: 8833.88,
    unitAmount: 4504.82,
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