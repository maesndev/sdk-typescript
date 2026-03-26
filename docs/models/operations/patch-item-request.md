# PatchItemRequest

## Example Usage

```typescript
import { PatchItemRequest } from "maesn/models/operations";

let value: PatchItemRequest = {
  itemId: "<id>",
  body: {
    name: "<value>",
    itemNumber: "<value>",
    stockCount: 9770.3,
    type: "SERVICE",
    unitName: "STÜCK",
    unitPurchasePrice: 8884.67,
    unitSalesPrice: 8802.04,
    priceIncludesTax: true,
  },
};
```

## Fields

| Field                                                                | Type                                                                 | Required                                                             | Description                                                          |
| -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------- |
| `itemId`                                                             | *string*                                                             | :heavy_check_mark:                                                   | N/A                                                                  |
| `environmentName`                                                    | *string*                                                             | :heavy_minus_sign:                                                   | N/A                                                                  |
| `companyId`                                                          | *string*                                                             | :heavy_minus_sign:                                                   | N/A                                                                  |
| `body`                                                               | [models.PatchItemRequestDto](../../models/patch-item-request-dto.md) | :heavy_check_mark:                                                   | N/A                                                                  |