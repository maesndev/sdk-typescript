# CreateSalesOrderRequest

## Example Usage

```typescript
import { CreateSalesOrderRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateSalesOrderRequest = {
  body: {},
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `environmentName`                                                                   | *string*                                                                            | :heavy_minus_sign:                                                                  | Environment name (required for multi-environment systems such as Business Central)  |
| `companyId`                                                                         | *string*                                                                            | :heavy_minus_sign:                                                                  | ID of the company (required for multi-company target systems)                       |
| `body`                                                                              | [models.CreateSalesOrderRequestDto](../../models/create-sales-order-request-dto.md) | :heavy_check_mark:                                                                  | N/A                                                                                 |