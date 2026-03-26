# CreatePaymentTermRequest

## Example Usage

```typescript
import { CreatePaymentTermRequest } from "maesn/models/operations";

let value: CreatePaymentTermRequest = {
  body: {
    code: "<value>",
    description: "secret wearily crossly sans phooey tenant fork sophisticated",
    discountDays: 8011.13,
    discountDays2: 4885.24,
    discountPercentage: 2710.64,
    discountPercentage2: 1512.1,
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
    paymentDays: 6191.69,
    paymentMethod: "<value>",
  },
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `companyId`                                                                           | *string*                                                                              | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `body`                                                                                | [models.CreatePaymentTermRequestDto](../../models/create-payment-term-request-dto.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |