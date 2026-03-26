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

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `invoiceId`                                                                   | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `lineItemId`                                                                  | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `environmentName`                                                             | *string*                                                                      | :heavy_minus_sign:                                                            | N/A                                                                           |
| `companyId`                                                                   | *string*                                                                      | :heavy_minus_sign:                                                            | N/A                                                                           |
| `body`                                                                        | [models.PatchLineItemRequestDto](../../models/patch-line-item-request-dto.md) | :heavy_check_mark:                                                            | N/A                                                                           |