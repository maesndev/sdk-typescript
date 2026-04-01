# GetBillLineItemsResponse

List of line items for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetBillLineItemsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetBillLineItemsResponse = {
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