# CreatePaymentTermResponse

## Example Usage

```typescript
import { CreatePaymentTermResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreatePaymentTermResponse = {
  data: {
    id: "<id>",
    code: "<value>",
    createdDate: "<value>",
    description: "when gee tighten vivid usable as personal tame ew",
    discountDays: 5351.22,
    discountDays2: 5765.19,
    discountPercentage: 8927.03,
    discountPercentage2: 3579.44,
    discountPeriods: [],
    dueType: "DUE_IN_DAYS",
    name: "<value>",
    paymentDays: 5253.98,
    paymentMethod: "AUTOMATIC_BANK_WITHDRAWAL",
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `meta`                                                                                         | [operations.CreatePaymentTermMeta](../../models/operations/create-payment-term-meta.md)        | :heavy_minus_sign:                                                                             | N/A                                                                                            |
| `data`                                                                                         | [models.PaymentTermResponseDto](../../models/payment-term-response-dto.md)                     | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `errors`                                                                                       | [operations.CreatePaymentTermErrors](../../models/operations/create-payment-term-errors.md)    | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `rawData`                                                                                      | [operations.CreatePaymentTermRawData](../../models/operations/create-payment-term-raw-data.md) | :heavy_check_mark:                                                                             | N/A                                                                                            |