# GetPurchaseOrderResponse

## Example Usage

```typescript
import { GetPurchaseOrderResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetPurchaseOrderResponse = {
  data: {
    id: "<id>",
    addresses: [
      {},
    ],
    approvalDate: "<value>",
    comment: null,
    createdDate: "<value>",
    currency: "PLN",
    description: "ew printer ouch privilege rudely above",
    lineItems: [],
    orderDate: "<value>",
    paymentTermId: "<id>",
    reference: "<value>",
    status: "OPEN",
    supplierId: "<id>",
    totalDiscountAmount: 9629.85,
    totalDiscountPercentage: 5129.62,
    totalGrossAmount: 1488.21,
    totalNetAmount: 8789.71,
    totalTaxAmount: 2704.94,
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `meta`                                                                                       | [operations.GetPurchaseOrderMeta](../../models/operations/get-purchase-order-meta.md)        | :heavy_minus_sign:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.PurchaseOrderResponseDto](../../models/purchase-order-response-dto.md)               | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.GetPurchaseOrderErrors](../../models/operations/get-purchase-order-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.GetPurchaseOrderRawData](../../models/operations/get-purchase-order-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |