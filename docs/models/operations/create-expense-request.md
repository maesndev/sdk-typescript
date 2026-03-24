# CreateExpenseRequest

## Example Usage

```typescript
import { CreateExpenseRequest } from "maesn/models/operations";

let value: CreateExpenseRequest = {
  body: {},
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `environmentName`                                                                             | *string*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `companyId`                                                                                   | *string*                                                                                      | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `xApiKey`                                                                                     | *string*                                                                                      | :heavy_minus_sign:                                                                            | API key                                                                                       |
| `xAccountKey`                                                                                 | *string*                                                                                      | :heavy_minus_sign:                                                                            | Account key                                                                                   |
| `body`                                                                                        | [operations.CreateExpenseRequestBody](../../models/operations/create-expense-request-body.md) | :heavy_check_mark:                                                                            | N/A                                                                                           |