# PatchItemRequest

## Example Usage

```typescript
import { PatchItemRequest } from "@maesn/typescript-sdk/models/operations";

let value: PatchItemRequest = {
  itemId: "<id>",
  body: {},
};
```

## Fields

| Field                                                                | Type                                                                 | Required                                                             | Description                                                          |
| -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- |
| `itemId`                                                             | *string*                                                             | :heavy_check_mark:                                                   | N/A                                                                  |
| `environmentName`                                                    | *string*                                                             | :heavy_minus_sign:                                                   | N/A                                                                  |
| `companyId`                                                          | *string*                                                             | :heavy_minus_sign:                                                   | N/A                                                                  |
| `body`                                                               | [models.PatchItemRequestDto](../../models/patch-item-request-dto.md) | :heavy_check_mark:                                                   | N/A                                                                  |