# PaymentTermResponseDto

## Example Usage

```typescript
import { PaymentTermResponseDto } from "@maesn/typescript-sdk/models";

let value: PaymentTermResponseDto = {
  id: "<id>",
  code: "<value>",
  createdDate: "<value>",
  description: "short-term doubtfully concerning",
  discountDays: 9514.8,
  discountDays2: 1301.78,
  discountDaysCalculation: "<value>",
  discountPercentage: 2822.43,
  discountPercentage2: 3290.27,
  discountPeriods: [
    {
      invoiceRange: "<value>",
      discountDeadline: null,
      discountDeadline2: "<value>",
      paymentDeadline: "<value>",
    },
  ],
  dueType: null,
  name: "<value>",
  paymentDays: 7429.33,
  paymentDaysCalculation: "<value>",
  paymentMethod: null,
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `id`                                                                                    | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `code`                                                                                  | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `createdDate`                                                                           | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `description`                                                                           | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `discountDays`                                                                          | *number*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `discountDays2`                                                                         | *number*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `discountDaysCalculation`                                                               | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `discountPercentage`                                                                    | *number*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `discountPercentage2`                                                                   | *number*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `discountPeriods`                                                                       | [models.DiscountPeriodResponse](../models/discount-period-response.md)[]                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `dueType`                                                                               | [models.PaymentTermResponseDtoDueType](../models/payment-term-response-dto-due-type.md) | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `name`                                                                                  | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `paymentDays`                                                                           | *number*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `paymentDaysCalculation`                                                                | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `paymentMethod`                                                                         | [models.PaymentMethod](../models/payment-method.md)                                     | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `updatedDate`                                                                           | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |