# CreateLineItemRequestDto

## Example Usage

```typescript
import { CreateLineItemRequestDto } from "maesn/models";

let value: CreateLineItemRequestDto = {
  accountCode: "<value>",
  accountId: "<id>",
  description: "whose beautifully via pish grounded without",
  dimensions: [
    {
      id: "<id>",
      categoryName: "<value>",
      name: "<value>",
    },
  ],
  discountItemPercentage: 912.85,
  grossAmount: 3084.07,
  itemId: "<id>",
  name: "<value>",
  quantity: 4558.06,
  taxCode: "<value>",
  taxRatePercentage: 9292.05,
  taxType: "<value>",
  type: "<value>",
  unitAmount: 8723.08,
  unitName: "<value>",
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `accountCode`                                                                     | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `accountId`                                                                       | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `description`                                                                     | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `dimensions`                                                                      | [models.InvoiceDimensionRequestDto](../models/invoice-dimension-request-dto.md)[] | :heavy_check_mark:                                                                | N/A                                                                               |
| `discountItemPercentage`                                                          | *number*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `grossAmount`                                                                     | *number*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `itemId`                                                                          | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `name`                                                                            | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `quantity`                                                                        | *number*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `taxCode`                                                                         | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `taxRatePercentage`                                                               | *number*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `taxType`                                                                         | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `type`                                                                            | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `unitAmount`                                                                      | *number*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `unitName`                                                                        | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |