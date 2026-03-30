# GetBillLineItemsResponse

List of line items for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetBillLineItemsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetBillLineItemsResponse = {
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

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `meta`                                                                                        | [operations.GetBillLineItemsMeta](../../models/operations/get-bill-line-items-meta.md)        | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `data`                                                                                        | [models.BillLineItemResponseDto](../../models/bill-line-item-response-dto.md)[]               | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `errors`                                                                                      | [operations.GetBillLineItemsErrors](../../models/operations/get-bill-line-items-errors.md)    | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `rawData`                                                                                     | [operations.GetBillLineItemsRawData](../../models/operations/get-bill-line-items-raw-data.md) | :heavy_check_mark:                                                                            | N/A                                                                                           |