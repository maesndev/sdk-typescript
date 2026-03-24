# GetPurchaseOrderResponse

## Example Usage

```typescript
import { GetPurchaseOrderResponse } from "maesn/models/operations";

let value: GetPurchaseOrderResponse = {
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
    approvalDate: "<value>",
    comment:
      "New ABC 13 9370, 13.3, 5th Gen CoreA5-8250U, 8GB RAM, 256GB SSD, power UHD Graphics, OS 10 Home, OS Office A & J 2016",
    createdDate: "<value>",
    currency: "SBD",
    description: "oof knottily sweet bonnet",
    lineItems: [],
    orderDate: "<value>",
    paymentTermId: "<id>",
    reference: "<value>",
    status: "<value>",
    supplierId: "<id>",
    totalDiscountAmount: 282.95,
    totalDiscountPercentage: 5610.59,
    totalGrossAmount: 5740.48,
    totalNetAmount: 5126.3,
    totalTaxAmount: 7075.83,
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
| `data`                                                                                       | [models.PurchaseOrderResponseDto](../../models/purchase-order-response-dto.md)               | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.GetPurchaseOrderErrors](../../models/operations/get-purchase-order-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.GetPurchaseOrderRawData](../../models/operations/get-purchase-order-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |