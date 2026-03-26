# GetPurchaseOrderLineItemResponse

## Example Usage

```typescript
import { GetPurchaseOrderLineItemResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetPurchaseOrderLineItemResponse = {
  data: {
    id: null,
    itemId: "<id>",
    createdDate: "<value>",
    description: "potentially if large husk minus gadzooks even aching",
    itemName: "<value>",
    quantity: 4098.93,
    taxCode: "<value>",
    taxRatePercentage: 1001.65,
    totalDiscountAmount: 3589.19,
    totalDiscountPercentage: 6508.66,
    totalGrossAmount: 2382.6,
    totalNetAmount: 6533.33,
    totalTaxAmount: 410.1,
    unitAmount: 7095.43,
    unitDiscountAmount: null,
    unitDiscountPercentage: 4478.25,
    unitName: "<value>",
    updatedDate: "<value>",
  },
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                                                          | Type                                                                                                           | Required                                                                                                       | Description                                                                                                    |
| -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                         | [operations.GetPurchaseOrderLineItemMeta](../../models/operations/get-purchase-order-line-item-meta.md)        | :heavy_minus_sign:                                                                                             | N/A                                                                                                            |
| `data`                                                                                                         | [models.PurchaseOrderLineItemResponseDto](../../models/purchase-order-line-item-response-dto.md)               | :heavy_check_mark:                                                                                             | N/A                                                                                                            |
| `errors`                                                                                                       | [operations.GetPurchaseOrderLineItemErrors](../../models/operations/get-purchase-order-line-item-errors.md)    | :heavy_check_mark:                                                                                             | N/A                                                                                                            |
| `rawData`                                                                                                      | [operations.GetPurchaseOrderLineItemRawData](../../models/operations/get-purchase-order-line-item-raw-data.md) | :heavy_check_mark:                                                                                             | N/A                                                                                                            |