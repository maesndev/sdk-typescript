# LineItemRequest

## Example Usage

```typescript
import { LineItemRequest } from "maesn/models";

let value: LineItemRequest = {
  id: "<id>",
  accountCode: "<value>",
  accountId: "<id>",
  accountName: "<value>",
  accountNumber: 7598.4,
  bookingTaxCode: "<value>",
  description: "safe poetry unusual excitable viciously yahoo abnormally bran",
  dimension1: "<value>",
  dimension2: "<value>",
  discountAmount: 4362.96,
  discountAmount2: 3140.84,
  discountPercentage: 5744.78,
  discountPercentage2: 7129.15,
  taxCode: "<value>",
  taxRatePercentage: 4341.26,
  totalGrossAmount: 2375.34,
  totalNetAmount: 4406.76,
  type: "GOODS",
};
```

## Fields

| Field                                                             | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `id`                                                              | *string*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `accountCode`                                                     | *string*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `accountId`                                                       | *string*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `accountName`                                                     | *string*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `accountNumber`                                                   | *number*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `bookingTaxCode`                                                  | *string*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `description`                                                     | *string*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `dimension1`                                                      | *string*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `dimension2`                                                      | *string*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `discountAmount`                                                  | *number*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `discountAmount2`                                                 | *number*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `discountPercentage`                                              | *number*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `discountPercentage2`                                             | *number*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `taxCode`                                                         | *string*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `taxRatePercentage`                                               | *number*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `totalGrossAmount`                                                | *number*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `totalNetAmount`                                                  | *number*                                                          | :heavy_check_mark:                                                | N/A                                                               |
| `type`                                                            | [models.LineItemRequestType](../models/line-item-request-type.md) | :heavy_check_mark:                                                | N/A                                                               |