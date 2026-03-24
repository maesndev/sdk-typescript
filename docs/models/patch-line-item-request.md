# PatchLineItemRequest

## Example Usage

```typescript
import { PatchLineItemRequest } from "maesn/models";

let value: PatchLineItemRequest = {
  lineItemId: "<id>",
  itemId: "<id>",
  unitName: "<value>",
  type: "TEXT",
  quantity: 9503.94,
  taxRatePercentage: 1919.78,
  unitAmount: 3883.73,
  grossAmount: 2088.78,
  taxCode: "<value>",
  taxType: "<value>",
  description: "unnaturally at yahoo fireplace",
  name: "<value>",
  accountCode: "<value>",
  accountId: "<id>",
  dimensions: [
    {
      id: "<id>",
      categoryName: "<value>",
      name: "<value>",
    },
  ],
  discountItemPercentage: 9430.13,
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `lineItemId`                                                                      | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `itemId`                                                                          | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `unitName`                                                                        | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `type`                                                                            | [models.PatchLineItemRequestType](../models/patch-line-item-request-type.md)      | :heavy_check_mark:                                                                | N/A                                                                               |
| `quantity`                                                                        | *number*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `taxRatePercentage`                                                               | *number*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `unitAmount`                                                                      | *number*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `grossAmount`                                                                     | *number*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `taxCode`                                                                         | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `taxType`                                                                         | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `description`                                                                     | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `name`                                                                            | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `accountCode`                                                                     | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `accountId`                                                                       | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `dimensions`                                                                      | [models.InvoiceDimensionRequestDto](../models/invoice-dimension-request-dto.md)[] | :heavy_check_mark:                                                                | N/A                                                                               |
| `discountItemPercentage`                                                          | *number*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |