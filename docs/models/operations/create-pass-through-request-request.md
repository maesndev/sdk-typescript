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
| `environmentName`                                                                     | *string*                                                                              | :heavy_minus_sign:                                                                    | Environment name (required for multi-environment systems such as Business Central)    |
| `companyId`                                                                           | *string*                                                                              | :heavy_minus_sign:                                                                    | ID of the company (required for multi-company target systems)                         |
| `body`                                                                                | [models.CreatePassThroughRequestDto](../../models/create-pass-through-request-dto.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |