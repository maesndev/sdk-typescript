# UpdateBillLineItemResponse

Bill line item updated successfully

## Example Usage

```typescript
import { UpdateBillLineItemResponse } from "@maesn/typescript-sdk/models/operations";

let value: UpdateBillLineItemResponse = {
  data: [
    {
      id: "<id>",
      accountId: "<id>",
      accountNumber: "<value>",
      createdDate: null,
      deferredEndDate: "<value>",
      deferredStartDate: "<value>",
      description:
        "since record muddy quintuple seafood hence likewise plumber ick ouch",
      dimensions: [
        {
          name: "<value>",
          categoryName: "<value>",
        },
      ],
      itemId: "<id>",
      itemName: "<value>",
      quantity: 1273.11,
      taxCode: null,
      taxRatePercentage: 248.32,
      totalDiscountAmount: 5210.72,
      totalDiscountPercentage: 7272.38,
      totalGrossAmount: 7810.47,
      totalNetAmount: 2983.23,
      totalTaxAmount: 3886.78,
      unitAmount: 632.5,
      unitDiscountAmount: null,
      unitDiscountPercentage: 2870.11,
      unitName: "<value>",
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                                             | Type                                                                                              | Required                                                                                          | Description                                                                                       |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `meta`                                                                                            | [operations.UpdateBillLineItemMeta](../../models/operations/update-bill-line-item-meta.md)        | :heavy_minus_sign:                                                                                | N/A                                                                                               |
| `data`                                                                                            | [models.BillLineItemResponseDto](../../models/bill-line-item-response-dto.md)[]                   | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `errors`                                                                                          | [operations.UpdateBillLineItemErrors](../../models/operations/update-bill-line-item-errors.md)    | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `rawData`                                                                                         | [operations.UpdateBillLineItemRawData](../../models/operations/update-bill-line-item-raw-data.md) | :heavy_check_mark:                                                                                | N/A                                                                                               |