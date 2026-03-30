# CreateExpenseRequest

## Example Usage

```typescript
import { CreateExpenseRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateExpenseRequest = {
  body: {},
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `environmentName`                                                                             | *string*                                                                                      | :heavy_minus_sign:                                                                            | Environment name (required for multi-environment systems such as Business Central)            |
| `companyId`                                                                                   | *string*                                                                                      | :heavy_minus_sign:                                                                            | ID of the company (required for multi-company target systems)                                 |
| `body`                                                                                        | [operations.CreateExpenseRequestBody](../../models/operations/create-expense-request-body.md) | :heavy_check_mark:                                                                            | N/A                                                                                           |