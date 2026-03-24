# CreatePaymentTermRequestDto

## Example Usage

```typescript
import { CreatePaymentTermRequestDto } from "maesn/models";

let value: CreatePaymentTermRequestDto = {
  code: "<value>",
  description:
    "after given violin breastplate than pace ultimate lecture stall",
  discountDays: 8799.16,
  discountDays2: 6265.01,
  discountPercentage: 4267.5,
  discountPercentage2: 5397.92,
  discountPeriods: [
    {
      invoiceRange: "<value>",
      discountDeadline: "<value>",
      discountDeadline2: "<value>",
      paymentDeadline: "<value>",
    },
  ],
  dueType: "DUE_IN_DAYS",
  name: "<value>",
  paymentDays: 298.18,
  paymentMethod: "<value>",
};
```

## Fields

| Field                                                                                              | Type                                                                                               | Required                                                                                           | Description                                                                                        |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| `code`                                                                                             | *string*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `description`                                                                                      | *string*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `discountDays`                                                                                     | *number*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `discountDays2`                                                                                    | *number*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `discountPercentage`                                                                               | *number*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `discountPercentage2`                                                                              | *number*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `discountPeriods`                                                                                  | [models.DiscountPeriodRequest](../models/discount-period-request.md)[]                             | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `dueType`                                                                                          | [models.CreatePaymentTermRequestDtoDueType](../models/create-payment-term-request-dto-due-type.md) | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `name`                                                                                             | *string*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `paymentDays`                                                                                      | *number*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `paymentMethod`                                                                                    | *string*                                                                                           | :heavy_check_mark:                                                                                 | N/A                                                                                                |