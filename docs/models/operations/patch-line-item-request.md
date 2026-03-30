# PatchLineItemRequest

## Example Usage

```typescript
import { PatchLineItemRequest } from "@maesn/typescript-sdk/models/operations";

let value: PatchLineItemRequest = {
  invoiceId: "<id>",
  lineItemId: "<id>",
  body: {},
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `invoiceId`                                                                        | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `lineItemId`                                                                       | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `body`                                                                             | [models.PatchLineItemRequestDto](../../models/patch-line-item-request-dto.md)      | :heavy_check_mark:                                                                 | N/A                                                                                |