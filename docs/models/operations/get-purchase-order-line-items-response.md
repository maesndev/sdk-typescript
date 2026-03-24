# GetPurchaseOrderLineItemsResponse

## Example Usage

```typescript
import { GetPurchaseOrderLineItemsResponse } from "maesn/models/operations";

let value: GetPurchaseOrderLineItemsResponse = {
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
      itemId: "<id>",
      createdDate: "<value>",
      description:
        "supposing likewise geez recklessly before oily hourly amid needily zowie",
      itemName: "<value>",
      quantity: 3448.91,
      taxCode: "<value>",
      taxRatePercentage: 995.56,
      totalDiscountAmount: 9296.23,
      totalDiscountPercentage: 7464.34,
      totalGrossAmount: 3023.94,
      totalNetAmount: 1347.36,
      totalTaxAmount: 7381.7,
      unitAmount: 8637.54,
      unitDiscountAmount: 1107.11,
      unitDiscountPercentage: 9589.99,
      unitName: "<value>",
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                            | Type                                                                                                             | Required                                                                                                         | Description                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                           | [models.MetaResponse](../../models/meta-response.md)                                                             | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `data`                                                                                                           | [models.PurchaseOrderLineItemResponseDto](../../models/purchase-order-line-item-response-dto.md)[]               | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `errors`                                                                                                         | [operations.GetPurchaseOrderLineItemsErrors](../../models/operations/get-purchase-order-line-items-errors.md)    | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `rawData`                                                                                                        | [operations.GetPurchaseOrderLineItemsRawData](../../models/operations/get-purchase-order-line-items-raw-data.md) | :heavy_check_mark:                                                                                               | N/A                                                                                                              |