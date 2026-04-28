# CreateTransactionRequest

## Example Usage

```typescript
import { CreateTransactionRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateTransactionRequest = {
  body: {},
};
```

## Fields

| Field                                                                                                 | Type                                                                                                  | Required                                                                                              | Description                                                                                           |
| ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| `companyId`                                                                                           | *string*                                                                                              | :heavy_minus_sign:                                                                                    | ID of the company (required for multi-company target systems)                                         |
| `apiKey`                                                                                              | *string*                                                                                              | :heavy_minus_sign:                                                                                    | API key                                                                                               |
| `accountKey`                                                                                          | *string*                                                                                              | :heavy_minus_sign:                                                                                    | Account key                                                                                           |
| `body`                                                                                                | [operations.CreateTransactionRequestBody](../../models/operations/create-transaction-request-body.md) | :heavy_check_mark:                                                                                    | N/A                                                                                                   |