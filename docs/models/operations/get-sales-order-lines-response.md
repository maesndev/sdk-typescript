# GetSalesOrderLinesResponse

## Example Usage

```typescript
import { GetSalesOrderLinesResponse } from "maesn/models/operations";

let value: GetSalesOrderLinesResponse = {
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
      description: "know gad boohoo playfully immediately frenetically",
      itemName: "<value>",
      quantity: 1477.83,
      taxCode: "<value>",
      taxRatePercentage: 7674.24,
      totalDiscountAmount: 5218.11,
      totalDiscountPercentage: 3707.45,
      totalGrossAmount: 5355.72,
      totalNetAmount: 799.83,
      totalTaxAmount: 8598.63,
      unitAmount: 4332.63,
      unitDiscountAmount: 9007.15,
      unitDiscountPercentage: 4.38,
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
| `data`                                                                                            | [models.SalesOrderLineItemResponseDto](../../models/sales-order-line-item-response-dto.md)[]      | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `errors`                                                                                          | [operations.GetSalesOrderLinesErrors](../../models/operations/get-sales-order-lines-errors.md)    | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `rawData`                                                                                         | [operations.GetSalesOrderLinesRawData](../../models/operations/get-sales-order-lines-raw-data.md) | :heavy_check_mark:                                                                                | N/A                                                                                               |