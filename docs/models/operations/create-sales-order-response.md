# CreateSalesOrderResponse

## Example Usage

```typescript
import { CreateSalesOrderResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateSalesOrderResponse = {
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
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `meta`                                                                                       | [operations.CreateSalesOrderMeta](../../models/operations/create-sales-order-meta.md)        | :heavy_minus_sign:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.SalesOrderResponseDto](../../models/sales-order-response-dto.md)                     | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.CreateSalesOrderErrors](../../models/operations/create-sales-order-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.CreateSalesOrderRawData](../../models/operations/create-sales-order-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |