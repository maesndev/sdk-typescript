# CreateContactV2Request

## Example Usage

```typescript
import { CreateContactV2Request } from "@maesn/typescript-sdk/models/operations";

let value: CreateContactV2Request = {
  body: {
    contactType: "COMPANY",
  },
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `environmentName`                                                                 | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `companyId`                                                                       | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `body`                                                                            | [models.CreateContactRequestDtoV2](../../models/create-contact-request-dto-v2.md) | :heavy_check_mark:                                                                | N/A                                                                               |