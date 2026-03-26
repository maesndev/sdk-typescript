# CreatePassThroughRequestRequest

## Example Usage

```typescript
import { CreatePassThroughRequestRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreatePassThroughRequestRequest = {
  body: {
    path: "/usr/include",
    method: "DELETE",
  },
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `environmentName`                                                                     | *string*                                                                              | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `companyId`                                                                           | *string*                                                                              | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `body`                                                                                | [models.CreatePassThroughRequestDto](../../models/create-pass-through-request-dto.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |