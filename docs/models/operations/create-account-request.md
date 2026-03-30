# CreateAccountRequest

## Example Usage

```typescript
import { CreateAccountRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateAccountRequest = {
  body: {},
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `body`                                                                             | [models.CreateAccountRequestDto](../../models/create-account-request-dto.md)       | :heavy_check_mark:                                                                 | N/A                                                                                |