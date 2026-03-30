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

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `body`                                                                             | [models.CreateContactRequestDtoV2](../../models/create-contact-request-dto-v2.md)  | :heavy_check_mark:                                                                 | N/A                                                                                |