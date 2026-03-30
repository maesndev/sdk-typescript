# GetPurchaseOrderLineItemsResponse

List of line items for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetPurchaseOrderLineItemsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetPurchaseOrderLineItemsResponse = {
  data: [
    {
      id: "<id>",
      itemId: "<id>",
      createdDate: "<value>",
      description: null,
      itemName: null,
      quantity: 1805.76,
      taxCode: "<value>",
      taxRatePercentage: 9314.4,
      totalDiscountAmount: 4661.33,
      totalDiscountPercentage: 481.18,
      totalGrossAmount: 3070.84,
      totalNetAmount: 908.82,
      totalTaxAmount: null,
      unitAmount: 6997.08,
      unitDiscountAmount: 4374.06,
      unitDiscountPercentage: 6811.34,
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
| `meta`                                                                                                           | [operations.GetPurchaseOrderLineItemsMeta](../../models/operations/get-purchase-order-line-items-meta.md)        | :heavy_minus_sign:                                                                                               | N/A                                                                                                              |
| `data`                                                                                                           | [models.PurchaseOrderLineItemResponseDto](../../models/purchase-order-line-item-response-dto.md)[]               | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `errors`                                                                                                         | [operations.GetPurchaseOrderLineItemsErrors](../../models/operations/get-purchase-order-line-items-errors.md)    | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `rawData`                                                                                                        | [operations.GetPurchaseOrderLineItemsRawData](../../models/operations/get-purchase-order-line-items-raw-data.md) | :heavy_check_mark:                                                                                               | N/A                                                                                                              |