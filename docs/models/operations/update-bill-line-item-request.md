# UpdateBillLineItemRequest

## Example Usage

```typescript
import { UpdateBillLineItemRequest } from "maesn/models/operations";

let value: UpdateBillLineItemRequest = {
  billId: "<id>",
  lineItemId: "<id>",
  body: {
    id: "<id>",
    accountId: "<id>",
    accountNumber: "<value>",
    deferredEndDate: "<value>",
    deferredStartDate: "<value>",
    description: "carefully soupy in puff kookily gah yum",
    dimensions: [],
    itemId: "<id>",
    itemName: "<value>",
    quantity: 8931.57,
    taxCode: "<value>",
    taxRatePercentage: 9228.58,
    totalDiscountAmount: 3530.68,
    totalDiscountPercentage: 5771.32,
    totalGrossAmount: 5979.3,
    totalNetAmount: 335.53,
    totalTaxAmount: 6527.52,
    unitAmount: 5239.62,
    unitDiscountAmount: 6441.36,
    unitDiscountPercentage: 9235.81,
    unitName: "<value>",
  },
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `billId`                                                                                 | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `lineItemId`                                                                             | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `companyId`                                                                              | *string*                                                                                 | :heavy_minus_sign:                                                                       | N/A                                                                                      |
| `body`                                                                                   | [models.CreateBillLineItemRequestDto](../../models/create-bill-line-item-request-dto.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |