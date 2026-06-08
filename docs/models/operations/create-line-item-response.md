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