# CreateTransactionRequest

## Example Usage

```typescript
import { CreateTransactionRequest } from "maesn/models/operations";

let value: CreateTransactionRequest = {
  body: {},
};
```

## Fields

| Field                                                                                                 | Type                                                                                                  | Required                                                                                              | Description                                                                                           |
| ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| `companyId`                                                                                           | *string*                                                                                              | :heavy_minus_sign:                                                                                    | N/A                                                                                                   |
| `xApiKey`                                                                                             | *string*                                                                                              | :heavy_minus_sign:                                                                                    | API key                                                                                               |
| `xAccountKey`                                                                                         | *string*                                                                                              | :heavy_minus_sign:                                                                                    | Account key                                                                                           |
| `body`                                                                                                | [operations.CreateTransactionRequestBody](../../models/operations/create-transaction-request-body.md) | :heavy_check_mark:                                                                                    | N/A                                                                                                   |