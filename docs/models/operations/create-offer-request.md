# CreateOfferRequest

## Example Usage

```typescript
import { CreateOfferRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateOfferRequest = {
  body: {
    addresses: [],
    currency: "Barbados Dollar",
    offerDate: "<value>",
  },
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `body`                                                                             | [models.CreateOfferRequestDto](../../models/create-offer-request-dto.md)           | :heavy_check_mark:                                                                 | N/A                                                                                |