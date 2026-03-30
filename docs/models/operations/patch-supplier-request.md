# PatchSupplierRequest

## Example Usage

```typescript
import { PatchSupplierRequest } from "@maesn/typescript-sdk/models/operations";

let value: PatchSupplierRequest = {
  contactId: "<id>",
  body: {},
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `contactId`                                                                        | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `body`                                                                             | [models.PatchContactRequestDto](../../models/patch-contact-request-dto.md)         | :heavy_check_mark:                                                                 | N/A                                                                                |