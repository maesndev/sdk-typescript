# CreateSupplierRequest

## Example Usage

```typescript
import { CreateSupplierRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateSupplierRequest = {
  body: {
    contactType: "COMPANY",
  },
};
```

## Fields

| Field                                                                        | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `environmentName`                                                            | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `companyId`                                                                  | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `body`                                                                       | [models.CreateContactRequestDto](../../models/create-contact-request-dto.md) | :heavy_check_mark:                                                           | N/A                                                                          |