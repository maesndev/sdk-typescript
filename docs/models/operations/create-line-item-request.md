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

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `invoiceId`                                                                     | *string*                                                                        | :heavy_check_mark:                                                              | N/A                                                                             |
| `environmentName`                                                               | *string*                                                                        | :heavy_minus_sign:                                                              | N/A                                                                             |
| `companyId`                                                                     | *string*                                                                        | :heavy_minus_sign:                                                              | N/A                                                                             |
| `body`                                                                          | [models.CreateLineItemRequestDto](../../models/create-line-item-request-dto.md) | :heavy_check_mark:                                                              | N/A                                                                             |