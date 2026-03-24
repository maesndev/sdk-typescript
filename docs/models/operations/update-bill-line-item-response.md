# UpdateBillLineItemResponse

## Example Usage

```typescript
import { UpdateBillLineItemResponse } from "maesn/models/operations";

let value: UpdateBillLineItemResponse = {
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
      accountId: "<id>",
      accountNumber: "<value>",
      createdDate: "<value>",
      deferredEndDate: "<value>",
      deferredStartDate: "<value>",
      description:
        "representation behind sedately anenst notwithstanding phooey diversity past",
      dimensions: [
        {
          name: "<value>",
          categoryName: "<value>",
        },
      ],
      itemId: "<id>",
      itemName: "<value>",
      quantity: 3634.11,
      taxCode: "<value>",
      taxRatePercentage: 3310.22,
      totalDiscountAmount: 707.82,
      totalDiscountPercentage: 4974.92,
      totalGrossAmount: 5058.37,
      totalNetAmount: 3913.59,
      totalTaxAmount: 2698.72,
      unitAmount: 9362.33,
      unitDiscountAmount: 9954.84,
      unitDiscountPercentage: 9564.66,
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
| `meta`                                                                                            | [models.MetaResponse](../../models/meta-response.md)                                              | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `data`                                                                                            | [models.BillLineItemResponseDto](../../models/bill-line-item-response-dto.md)[]                   | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `errors`                                                                                          | [operations.UpdateBillLineItemErrors](../../models/operations/update-bill-line-item-errors.md)    | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `rawData`                                                                                         | [operations.UpdateBillLineItemRawData](../../models/operations/update-bill-line-item-raw-data.md) | :heavy_check_mark:                                                                                | N/A                                                                                               |