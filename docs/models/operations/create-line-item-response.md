# CreateLineItemResponse

Line item created successfully

## Example Usage

```typescript
import { CreateLineItemResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateLineItemResponse = {
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
  rawData: {},
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `meta`                                                                                   | [operations.CreateLineItemMeta](../../models/operations/create-line-item-meta.md)        | :heavy_minus_sign:                                                                       | N/A                                                                                      |
| `data`                                                                                   | [models.LineItemResponseDto](../../models/line-item-response-dto.md)                     | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `errors`                                                                                 | [operations.CreateLineItemErrors](../../models/operations/create-line-item-errors.md)    | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `rawData`                                                                                | [operations.CreateLineItemRawData](../../models/operations/create-line-item-raw-data.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |