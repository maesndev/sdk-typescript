# GetSalesOrderResponse

Sales order record matching the provided ID

## Example Usage

```typescript
import { GetSalesOrderResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetSalesOrderResponse = {
  data: {
    id: "<id>",
    addresses: null,
    billingContactId: "<id>",
    comment:
      "New ABC 13 9370, 13.3, 5th Gen CoreA5-8250U, 8GB RAM, 256GB SSD, power UHD Graphics, OS 10 Home, OS Office A & J 2016",
    contactId: "<id>",
    createdDate: "<value>",
    currency: null,
    deliveryDate: "<value>",
    lineItems: null,
    orderDate: "<value>",
    projectId: "<id>",
    shippingContactId: "<id>",
    status: "OPEN",
    taskId: "<id>",
    totalDiscountAmount: 3105.59,
    totalDiscountPercentage: 6467.42,
    totalGrossAmount: 5424.24,
    totalNetAmount: null,
    totalTaxAmount: 4026.96,
    updatedDate: "<value>",
  },
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `meta`                                                                                 | [operations.GetSalesOrderMeta](../../models/operations/get-sales-order-meta.md)        | :heavy_minus_sign:                                                                     | N/A                                                                                    |
| `data`                                                                                 | [models.SalesOrderResponseDto](../../models/sales-order-response-dto.md)               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `errors`                                                                               | [operations.GetSalesOrderErrors](../../models/operations/get-sales-order-errors.md)    | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `rawData`                                                                              | [operations.GetSalesOrderRawData](../../models/operations/get-sales-order-raw-data.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |