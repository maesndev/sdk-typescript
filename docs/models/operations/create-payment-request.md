# CreatePaymentRequest

## Example Usage

```typescript
import { CreatePaymentRequest } from "maesn/models/operations";

let value: CreatePaymentRequest = {
  body: {
    currency: "Tugrik",
    documentType: "<value>",
    exchangeRate: 5239.43,
    journalCode: "<value>",
    paymentType: "<value>",
    paymentLines: [],
  },
};
```

## Fields

| Field                                                                        | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `companyId`                                                                  | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `xApiKey`                                                                    | *string*                                                                     | :heavy_minus_sign:                                                           | API key                                                                      |
| `xAccountKey`                                                                | *string*                                                                     | :heavy_minus_sign:                                                           | Account key                                                                  |
| `body`                                                                       | [models.CreatePaymentRequestDto](../../models/create-payment-request-dto.md) | :heavy_check_mark:                                                           | N/A                                                                          |