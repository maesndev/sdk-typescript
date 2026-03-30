# CreateLineItemRequest

## Example Usage

```typescript
import { CreateLineItemRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateLineItemRequest = {
  invoiceId: "<id>",
  body: {
    quantity: 4059.96,
  },
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `invoiceId`                                                                        | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `body`                                                                             | [models.CreateLineItemRequestDto](../../models/create-line-item-request-dto.md)    | :heavy_check_mark:                                                                 | N/A                                                                                |