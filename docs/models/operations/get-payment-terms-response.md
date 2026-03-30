# GetPaymentTermsResponse

List of payment terms for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetPaymentTermsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetPaymentTermsResponse = {
  data: [
    {
      id: "<id>",
      code: "<value>",
      createdDate: "<value>",
      description: "in surprisingly which",
      discountDays: 9183.45,
      discountDays2: 5849.96,
      discountPercentage: 8706.72,
      discountPercentage2: null,
      discountPeriods: [
        {
          invoiceRange: null,
          discountDeadline: "<value>",
          discountDeadline2: "<value>",
          paymentDeadline: "<value>",
        },
      ],
      dueType: "DUE_IN_DAYS",
      name: "<value>",
      paymentDays: 9240.36,
      paymentMethod: null,
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `meta`                                                                                     | [operations.GetPaymentTermsMeta](../../models/operations/get-payment-terms-meta.md)        | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.PaymentTermResponseDto](../../models/payment-term-response-dto.md)[]               | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.GetPaymentTermsErrors](../../models/operations/get-payment-terms-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.GetPaymentTermsRawData](../../models/operations/get-payment-terms-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |