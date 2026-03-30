# CreatePaymentRequest

## Example Usage

```typescript
import { CreatePaymentRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreatePaymentRequest = {
  body: {},
};
```

## Fields

| Field                                                                        | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `companyId`                                                                  | *string*                                                                     | :heavy_minus_sign:                                                           | ID of the company (required for multi-company target systems)                |
| `body`                                                                       | [models.CreatePaymentRequestDto](../../models/create-payment-request-dto.md) | :heavy_check_mark:                                                           | N/A                                                                          |