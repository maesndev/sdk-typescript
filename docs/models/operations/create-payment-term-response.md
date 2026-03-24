# CreatePaymentTermResponse

## Example Usage

```typescript
import { CreatePaymentTermResponse } from "maesn/models/operations";

let value: CreatePaymentTermResponse = {
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
    code: "<value>",
    createdDate: "<value>",
    description:
      "emotional minus manipulate how provided aware qua acknowledge tabletop amidst",
    discountDays: 5765.19,
    discountDays2: 5766.81,
    discountPercentage: 8927.03,
    discountPercentage2: 8017.5,
    discountPeriods: [],
    dueType: "DUE_AS_PERIOD",
    name: "<value>",
    paymentDays: 2807.76,
    paymentMethod: "<value>",
    updatedDate: {},
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `meta`                                                                                         | [models.MetaResponse](../../models/meta-response.md)                                           | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `data`                                                                                         | [models.PaymentTermResponseDto](../../models/payment-term-response-dto.md)                     | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `errors`                                                                                       | [operations.CreatePaymentTermErrors](../../models/operations/create-payment-term-errors.md)    | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `rawData`                                                                                      | [operations.CreatePaymentTermRawData](../../models/operations/create-payment-term-raw-data.md) | :heavy_check_mark:                                                                             | N/A                                                                                            |