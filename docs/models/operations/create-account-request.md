# CreateAccountRequest

## Example Usage

```typescript
import { CreateAccountRequest } from "maesn/models/operations";

let value: CreateAccountRequest = {
  body: {
    balance: 7456.97,
    class: "EXPENSE",
    code: "<value>",
    currency: "GQE",
    description: "stable meanwhile meanwhile",
    name: "<value>",
    number: "<value>",
    parentAccountId: "<id>",
    status: "ARCHIVED",
    type: "EXCHANGE_RATE_EXPENSE",
  },
};
```

## Fields

| Field                                                                        | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `environmentName`                                                            | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `companyId`                                                                  | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `body`                                                                       | [models.CreateAccountRequestDto](../../models/create-account-request-dto.md) | :heavy_check_mark:                                                           | N/A                                                                          |