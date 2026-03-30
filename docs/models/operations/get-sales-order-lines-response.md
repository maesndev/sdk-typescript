# GetSalesOrderLinesResponse

List of line items for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetSalesOrderLinesResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetSalesOrderLinesResponse = {
  data: [
    {
      id: "<id>",
      itemId: "<id>",
      createdDate: "<value>",
      description: "pension celebrated outlaw",
      itemName: null,
      quantity: 5836.18,
      taxCode: "<value>",
      taxRatePercentage: 4897.41,
      totalDiscountAmount: 7508.81,
      totalDiscountPercentage: 3465.64,
      totalGrossAmount: 5882.34,
      totalNetAmount: 1291.77,
      totalTaxAmount: 4110.59,
      unitAmount: 1477.83,
      unitDiscountAmount: 5218.11,
      unitDiscountPercentage: 5355.72,
      unitName: null,
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
| `meta`                                                                                            | [operations.GetSalesOrderLinesMeta](../../models/operations/get-sales-order-lines-meta.md)        | :heavy_minus_sign:                                                                                | N/A                                                                                               |
| `data`                                                                                            | [models.SalesOrderLineItemResponseDto](../../models/sales-order-line-item-response-dto.md)[]      | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `errors`                                                                                          | [operations.GetSalesOrderLinesErrors](../../models/operations/get-sales-order-lines-errors.md)    | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `rawData`                                                                                         | [operations.GetSalesOrderLinesRawData](../../models/operations/get-sales-order-lines-raw-data.md) | :heavy_check_mark:                                                                                | N/A                                                                                               |