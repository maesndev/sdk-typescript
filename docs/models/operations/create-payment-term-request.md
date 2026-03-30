# CreatePaymentTermRequest

## Example Usage

```typescript
import { CreatePaymentTermRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreatePaymentTermRequest = {
  body: {},
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `companyId`                                                                           | *string*                                                                              | :heavy_minus_sign:                                                                    | ID of the company (required for multi-company target systems)                         |
| `body`                                                                                | [models.CreatePaymentTermRequestDto](../../models/create-payment-term-request-dto.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |