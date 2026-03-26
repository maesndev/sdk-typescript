# UpdateSupplierRequest

## Example Usage

```typescript
import { UpdateSupplierRequest } from "@maesn/typescript-sdk/models/operations";

let value: UpdateSupplierRequest = {
  contactId: "<id>",
  body: {
    contactType: "COMPANY",
  },
};
```

## Fields

| Field                                                                        | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `contactId`                                                                  | *string*                                                                     | :heavy_check_mark:                                                           | N/A                                                                          |
| `companyId`                                                                  | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `body`                                                                       | [models.CreateContactRequestDto](../../models/create-contact-request-dto.md) | :heavy_check_mark:                                                           | N/A                                                                          |