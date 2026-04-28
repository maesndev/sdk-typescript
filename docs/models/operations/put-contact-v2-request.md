# PutContactV2Request

## Example Usage

```typescript
import { PutContactV2Request } from "@maesn/typescript-sdk/models/operations";

let value: PutContactV2Request = {
  contactId: "<id>",
  body: {
    contactType: "COMPANY",
  },
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `contactId`                                                                        | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `apiKey`                                                                           | *string*                                                                           | :heavy_minus_sign:                                                                 | API key                                                                            |
| `accountKey`                                                                       | *string*                                                                           | :heavy_minus_sign:                                                                 | Account key                                                                        |
| `body`                                                                             | [models.CreateContactRequestDtoV2](../../models/create-contact-request-dto-v2.md)  | :heavy_check_mark:                                                                 | N/A                                                                                |