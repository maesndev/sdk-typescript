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
| `environmentName`                                                                       | *string*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `companyId`                                                                             | *string*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `body`                                                                                  | [models.CreateVendorCreditRequestDto](../../models/create-vendor-credit-request-dto.md) | :heavy_check_mark:                                                                      | N/A                                                                                     |