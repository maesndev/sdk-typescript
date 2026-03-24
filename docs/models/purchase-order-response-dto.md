# PurchaseOrderResponseDto

## Example Usage

```typescript
import { PurchaseOrderResponseDto } from "maesn/models";

let value: PurchaseOrderResponseDto = {
  id: "<id>",
  addresses: [],
  approvalDate: "<value>",
  comment:
    "The beautiful range of Apple Naturalé that has an exciting mix of natural ingredients. With the Goodness of 100% Natural Ingredients",
  createdDate: "<value>",
  currency: "MAD",
  description: "disposer deserted disappointment which graceful nautical nor",
  lineItems: [],
  orderDate: "<value>",
  paymentTermId: "<id>",
  reference: "<value>",
  status: "<value>",
  supplierId: "<id>",
  totalDiscountAmount: 4339.04,
  totalDiscountPercentage: 6245.03,
  totalGrossAmount: 6507.73,
  totalNetAmount: 1847.36,
  totalTaxAmount: 8152.57,
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `id`                                                                                            | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `addresses`                                                                                     | [models.Address](../models/address.md)[]                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `approvalDate`                                                                                  | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `comment`                                                                                       | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `createdDate`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `currency`                                                                                      | [models.PurchaseOrderResponseDtoCurrency](../models/purchase-order-response-dto-currency.md)    | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `description`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `lineItems`                                                                                     | [models.PurchaseOrderLineItemResponseDto](../models/purchase-order-line-item-response-dto.md)[] | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `orderDate`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paymentTermId`                                                                                 | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `reference`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `status`                                                                                        | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `supplierId`                                                                                    | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalDiscountAmount`                                                                           | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalDiscountPercentage`                                                                       | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalGrossAmount`                                                                              | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalNetAmount`                                                                                | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `totalTaxAmount`                                                                                | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `updatedDate`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |