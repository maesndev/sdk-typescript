# PatchLineItemRequest

## Example Usage

```typescript
import { PatchLineItemRequest } from "maesn/models/operations";

let value: PatchLineItemRequest = {
  invoiceId: "<id>",
  lineItemId: "<id>",
  body: {
    accountCode: "<value>",
    description: "unless badly instead goose wavy competent afore lift faint",
    discountItemPercentage: 1925.09,
    grossAmount: 6707.76,
    itemId: "<id>",
    name: "<value>",
    quantity: 5991.11,
    taxCode: "<value>",
    taxRatePercentage: 4126.73,
    taxType: "<value>",
    type: "MATERIAL",
    unitAmount: 7214.53,
    unitName: "<value>",
  },
};
```

## Fields

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `invoiceId`                                                                   | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `lineItemId`                                                                  | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `environmentName`                                                             | *string*                                                                      | :heavy_minus_sign:                                                            | N/A                                                                           |
| `companyId`                                                                   | *string*                                                                      | :heavy_minus_sign:                                                            | N/A                                                                           |
| `body`                                                                        | [models.PatchLineItemRequestDto](../../models/patch-line-item-request-dto.md) | :heavy_check_mark:                                                            | N/A                                                                           |