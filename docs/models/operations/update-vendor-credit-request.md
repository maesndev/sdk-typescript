# UpdateVendorCreditRequest

## Example Usage

```typescript
import { UpdateVendorCreditRequest } from "@maesn/typescript-sdk/models/operations";

let value: UpdateVendorCreditRequest = {
  vendorCreditId: "<id>",
  body: {
    vendorCreditDate: "<value>",
    vendorCreditNumber: "<value>",
  },
};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `vendorCreditId`                                                                        | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `environmentName`                                                                       | *string*                                                                                | :heavy_minus_sign:                                                                      | Environment name (required for multi-environment systems such as Business Central)      |
| `companyId`                                                                             | *string*                                                                                | :heavy_minus_sign:                                                                      | ID of the company (required for multi-company target systems)                           |
| `apiKey`                                                                                | *string*                                                                                | :heavy_minus_sign:                                                                      | API key                                                                                 |
| `accountKey`                                                                            | *string*                                                                                | :heavy_minus_sign:                                                                      | Account key                                                                             |
| `body`                                                                                  | [models.CreateVendorCreditRequestDto](../../models/create-vendor-credit-request-dto.md) | :heavy_check_mark:                                                                      | N/A                                                                                     |