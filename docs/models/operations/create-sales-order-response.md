# CreateSalesOrderResponse

## Example Usage

```typescript
import { CreateSalesOrderResponse } from "maesn/models/operations";

let value: CreateSalesOrderResponse = {
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
  data: {
    id: "<id>",
    addresses: [
      {
        addressLine1: "429 Walsh Tunnel",
        addressLine2: "-",
        city: "East Melyssa",
        countryCode: "AE",
        postalCode: "39193",
        type: "SELLING",
      },
    ],
    billingContactId: "<id>",
    comment:
      "Andy shoes are designed to keeping in mind durability as well as trends, the most stylish range of shoes & sandals",
    contactId: "<id>",
    createdDate: "<value>",
    currency: "Lebanese Pound",
    deliveryDate: "<value>",
    lineItems: [
      {
        id: "<id>",
        itemId: "<id>",
        createdDate: "<value>",
        description: "why save per eyebrow regulate",
        itemName: "<value>",
        quantity: 5076.03,
        taxCode: "<value>",
        taxRatePercentage: 1241.75,
        totalDiscountAmount: 7988.4,
        totalDiscountPercentage: 7646.56,
        totalGrossAmount: 5584.87,
        totalNetAmount: 1492.5,
        totalTaxAmount: 4302.98,
        unitAmount: 5856.61,
        unitDiscountAmount: 4921.26,
        unitDiscountPercentage: 1866.03,
        unitName: "<value>",
        updatedDate: "<value>",
      },
    ],
    oneLineAddress: "<value>",
    orderDate: "<value>",
    projectId: "<id>",
    shippingContactId: "<id>",
    status: "VOIDED",
    taskId: "<id>",
    totalDiscountAmount: 2521.55,
    totalDiscountPercentage: 5656.09,
    totalGrossAmount: 9513.8,
    totalNetAmount: 1524.59,
    totalTaxAmount: 6295.98,
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `meta`                                                                                       | [models.MetaResponse](../../models/meta-response.md)                                         | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.SalesOrderResponseDto](../../models/sales-order-response-dto.md)                     | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.CreateSalesOrderErrors](../../models/operations/create-sales-order-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.CreateSalesOrderRawData](../../models/operations/create-sales-order-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |