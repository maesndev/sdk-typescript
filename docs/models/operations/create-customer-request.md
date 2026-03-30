# CreateCustomerRequest

## Example Usage

```typescript
import { CreateCustomerRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateCustomerRequest = {
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
| `body`                                                                             | [models.CreateContactRequestDto](../../models/create-contact-request-dto.md)       | :heavy_check_mark:                                                                 | N/A                                                                                |