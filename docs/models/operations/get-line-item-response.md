# GetLineItemResponse

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

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `meta`                                                                             | [operations.GetLineItemMeta](../../models/operations/get-line-item-meta.md)        | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `data`                                                                             | [models.LineItemResponseDto](../../models/line-item-response-dto.md)               | :heavy_check_mark:                                                                 | N/A                                                                                |
| `errors`                                                                           | [operations.GetLineItemErrors](../../models/operations/get-line-item-errors.md)    | :heavy_check_mark:                                                                 | N/A                                                                                |
| `rawData`                                                                          | [operations.GetLineItemRawData](../../models/operations/get-line-item-raw-data.md) | :heavy_check_mark:                                                                 | N/A                                                                                |