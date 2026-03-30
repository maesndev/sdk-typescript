# CreateBankAccountRequest

## Example Usage

```typescript
import { CreateBankAccountRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateBankAccountRequest = {
  body: {},
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `environmentName`                                                                     | *string*                                                                              | :heavy_minus_sign:                                                                    | Environment name (required for multi-environment systems such as Business Central)    |
| `companyId`                                                                           | *string*                                                                              | :heavy_minus_sign:                                                                    | ID of the company (required for multi-company target systems)                         |
| `body`                                                                                | [models.CreateBankAccountRequestDto](../../models/create-bank-account-request-dto.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |