# GetPaymentTermsResponse

## Example Usage

```typescript
import { GetPaymentTermsResponse } from "maesn/models/operations";

let value: GetPaymentTermsResponse = {
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
  data: [
    {
      id: "<id>",
      code: "<value>",
      createdDate: "<value>",
      description:
        "shush tall considering given and gosh CD lest liberalize incidentally",
      discountDays: 458.02,
      discountDays2: 7860.02,
      discountPercentage: 8027.97,
      discountPercentage2: 6352.07,
      discountPeriods: [
        {
          invoiceRange: "<value>",
          discountDeadline: "<value>",
          discountDeadline2: "<value>",
          paymentDeadline: "<value>",
        },
      ],
      dueType: "DUE_AS_PERIOD",
      name: "<value>",
      paymentDays: 8505.52,
      paymentMethod: "<value>",
      updatedDate: {},
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `meta`                                                                                     | [models.MetaResponse](../../models/meta-response.md)                                       | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.PaymentTermResponseDto](../../models/payment-term-response-dto.md)[]               | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.GetPaymentTermsErrors](../../models/operations/get-payment-terms-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.GetPaymentTermsRawData](../../models/operations/get-payment-terms-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |