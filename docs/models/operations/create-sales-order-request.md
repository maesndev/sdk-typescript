# CreateSalesOrderRequest

## Example Usage

```typescript
import { CreateSalesOrderRequest } from "maesn/models/operations";

let value: CreateSalesOrderRequest = {
  body: {
    addresses: [],
    billingContactId: "<id>",
    comment:
      "The Apollotech B340 is an affordable wireless mouse with reliable connectivity, 12 months battery life and modern design",
    contactId: "<id>",
    currency: "Leone",
    deliveryDate: "<value>",
    lineItems: [],
    oneLineAddress: "<value>",
    orderDate: "<value>",
    projectId: "<id>",
    shippingContactId: "<id>",
    status: "IN_REVIEW",
    totalDiscountAmount: 2665.86,
    totalDiscountPercentage: 2098.39,
    totalGrossAmount: 53.67,
    totalNetAmount: 7757.21,
    totalTaxAmount: 6786.28,
    version: "<value>",
  },
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `environmentName`                                                                   | *string*                                                                            | :heavy_minus_sign:                                                                  | N/A                                                                                 |
| `companyId`                                                                         | *string*                                                                            | :heavy_minus_sign:                                                                  | N/A                                                                                 |
| `xApiKey`                                                                           | *string*                                                                            | :heavy_minus_sign:                                                                  | API key                                                                             |
| `xAccountKey`                                                                       | *string*                                                                            | :heavy_minus_sign:                                                                  | Account key                                                                         |
| `body`                                                                              | [models.CreateSalesOrderRequestDto](../../models/create-sales-order-request-dto.md) | :heavy_check_mark:                                                                  | N/A                                                                                 |