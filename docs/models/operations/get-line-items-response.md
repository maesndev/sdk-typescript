# GetLineItemsResponse

## Example Usage

```typescript
import { GetLineItemsResponse } from "maesn/models/operations";

let value: GetLineItemsResponse = {
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
      lineItemId: "<id>",
      accountId: "<id>",
      createdDate: {},
      description: "notwithstanding bookend lovingly slide till as",
      dimensions: [
        {
          id: "<id>",
          categoryName: "<value>",
          name: "<value>",
        },
      ],
      discountItemAmount: 9973.62,
      discountItemPercentage: 3508.6,
      grossAmount: 6692.06,
      itemsAmount: 4105.84,
      itemId: "<id>",
      name: "<value>",
      quantity: 3109.42,
      taxCode: "<value>",
      taxRatePercentage: 2190.73,
      unitAmount: 619.76,
      updatedDate: {},
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                | Type                                                                                 | Required                                                                             | Description                                                                          |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| `meta`                                                                               | [models.MetaResponse](../../models/meta-response.md)                                 | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `data`                                                                               | [models.LineItemResponseDto](../../models/line-item-response-dto.md)[]               | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `errors`                                                                             | [operations.GetLineItemsErrors](../../models/operations/get-line-items-errors.md)    | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `rawData`                                                                            | [operations.GetLineItemsRawData](../../models/operations/get-line-items-raw-data.md) | :heavy_check_mark:                                                                   | N/A                                                                                  |