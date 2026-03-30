# UpdateBillLineItemResponse

Bill line item updated successfully

## Example Usage

```typescript
import { UpdateBillLineItemResponse } from "@maesn/typescript-sdk/models/operations";

let value: UpdateBillLineItemResponse = {
  data: [
    {
      id: "<id>",
      accountId: null,
      accountNumber: "<value>",
      createdDate: "<value>",
      deferredEndDate: "<value>",
      deferredStartDate: "<value>",
      description:
        "behind sedately anenst notwithstanding phooey diversity past aha",
      dimensions: [
        {
          name: "<value>",
          categoryName: "<value>",
        },
      ],
      itemId: "<id>",
      itemName: "<value>",
      quantity: 972.26,
      taxCode: null,
      taxRatePercentage: 7368.09,
      totalDiscountAmount: 6048.94,
      totalDiscountPercentage: 7206.62,
      totalGrossAmount: 7285.99,
      totalNetAmount: 2328.6,
      totalTaxAmount: 5246.18,
      unitAmount: 7884.58,
      unitDiscountAmount: 5739.68,
      unitDiscountPercentage: 5524.06,
      unitName: "<value>",
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                             | Type                                                                                              | Required                                                                                          | Description                                                                                       |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `meta`                                                                                            | [operations.UpdateBillLineItemMeta](../../models/operations/update-bill-line-item-meta.md)        | :heavy_minus_sign:                                                                                | N/A                                                                                               |
| `data`                                                                                            | [models.BillLineItemResponseDto](../../models/bill-line-item-response-dto.md)[]                   | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `errors`                                                                                          | [operations.UpdateBillLineItemErrors](../../models/operations/update-bill-line-item-errors.md)    | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `rawData`                                                                                         | [operations.UpdateBillLineItemRawData](../../models/operations/update-bill-line-item-raw-data.md) | :heavy_check_mark:                                                                                | N/A                                                                                               |