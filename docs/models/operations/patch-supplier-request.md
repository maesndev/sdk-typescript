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

| Field                                                                      | Type                                                                       | Required                                                                   | Description                                                                |
| -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| `contactId`                                                                | *string*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `environmentName`                                                          | *string*                                                                   | :heavy_minus_sign:                                                         | N/A                                                                        |
| `companyId`                                                                | *string*                                                                   | :heavy_minus_sign:                                                         | N/A                                                                        |
| `body`                                                                     | [models.PatchContactRequestDto](../../models/patch-contact-request-dto.md) | :heavy_check_mark:                                                         | N/A                                                                        |