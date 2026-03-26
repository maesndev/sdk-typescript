# PatchContactRequest

## Example Usage

```typescript
import { PatchContactRequest } from "@maesn/typescript-sdk/models/operations";

let value: PatchContactRequest = {
  contactId: "<id>",
  body: {
    contactType: "COMPANY",
  },
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `contactId`                                                                       | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `environmentName`                                                                 | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `companyId`                                                                       | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `body`                                                                            | [models.CreateContactRequestDtoV2](../../models/create-contact-request-dto-v2.md) | :heavy_check_mark:                                                                | N/A                                                                               |