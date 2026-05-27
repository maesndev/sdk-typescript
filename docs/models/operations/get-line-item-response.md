# GetLineItemResponse

Line item record matching the provided ID

## Example Usage

```typescript
import { GetLineItemResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetLineItemResponse = {
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
    taxRatePercentage: 7045.2,
    unitAmount: 6084.94,
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `meta`                                                                             | [operations.GetLineItemMeta](../../models/operations/get-line-item-meta.md)        | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `data`                                                                             | [models.LineItemResponseDto](../../models/line-item-response-dto.md)               | :heavy_check_mark:                                                                 | N/A                                                                                |
| `errors`                                                                           | [operations.GetLineItemErrors](../../models/operations/get-line-item-errors.md)    | :heavy_check_mark:                                                                 | N/A                                                                                |
| `rawData`                                                                          | [operations.GetLineItemRawData](../../models/operations/get-line-item-raw-data.md) | :heavy_check_mark:                                                                 | N/A                                                                                |