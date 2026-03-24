# PaymentTermResponseDto

## Example Usage

```typescript
import { PaymentTermResponseDto } from "maesn/models";

let value: PaymentTermResponseDto = {
  id: "<id>",
  code: "<value>",
  createdDate: "<value>",
  description: "though joyful poorly between",
  discountDays: 1301.78,
  discountDays2: 3257.64,
  discountPercentage: 3732.23,
  discountPercentage2: 2822.43,
  discountPeriods: [],
  dueType: "DUE_IN_DAYS",
  name: "<value>",
  paymentDays: 3647.65,
  paymentMethod: "<value>",
  updatedDate: {},
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `id`                                                                                            | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `code`                                                                                          | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `createdDate`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `description`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `discountDays`                                                                                  | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `discountDays2`                                                                                 | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `discountPercentage`                                                                            | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `discountPercentage2`                                                                           | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `discountPeriods`                                                                               | [models.DiscountPeriodResponse](../models/discount-period-response.md)[]                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `dueType`                                                                                       | [models.PaymentTermResponseDtoDueType](../models/payment-term-response-dto-due-type.md)         | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `name`                                                                                          | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paymentDays`                                                                                   | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `paymentMethod`                                                                                 | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `updatedDate`                                                                                   | [models.PaymentTermResponseDtoUpdatedDate](../models/payment-term-response-dto-updated-date.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |