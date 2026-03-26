# CreateVendorCreditRequest

## Example Usage

```typescript
import { CreateVendorCreditRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateVendorCreditRequest = {
  body: {
    vendorCreditDate: "<value>",
    vendorCreditNumber: "<value>",
  },
};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `environmentName`                                                                       | *string*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `companyId`                                                                             | *string*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `body`                                                                                  | [models.CreateVendorCreditRequestDto](../../models/create-vendor-credit-request-dto.md) | :heavy_check_mark:                                                                      | N/A                                                                                     |