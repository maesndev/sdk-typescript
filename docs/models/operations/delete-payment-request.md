# DeletePaymentRequest

## Example Usage

```typescript
import { DeletePaymentRequest } from "@maesn/typescript-sdk/models/operations";

let value: DeletePaymentRequest = {
  paymentId: "<id>",
};
```

## Fields

| Field                                                         | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `paymentId`                                                   | *string*                                                      | :heavy_check_mark:                                            | N/A                                                           |
| `companyId`                                                   | *string*                                                      | :heavy_minus_sign:                                            | ID of the company (required for multi-company target systems) |
| `apiKey`                                                      | *string*                                                      | :heavy_minus_sign:                                            | API key                                                       |
| `accountKey`                                                  | *string*                                                      | :heavy_minus_sign:                                            | Account key                                                   |