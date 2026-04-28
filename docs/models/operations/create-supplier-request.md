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

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `apiKey`                                                                           | *string*                                                                           | :heavy_minus_sign:                                                                 | API key                                                                            |
| `accountKey`                                                                       | *string*                                                                           | :heavy_minus_sign:                                                                 | Account key                                                                        |
| `body`                                                                             | [models.CreateContactRequestDto](../../models/create-contact-request-dto.md)       | :heavy_check_mark:                                                                 | N/A                                                                                |