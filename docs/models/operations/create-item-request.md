# CreateItemRequest

## Example Usage

```typescript
import { CreateItemRequest } from "maesn/models/operations";

let value: CreateItemRequest = {
  body: {
    assetAccountId: "<id>",
    expenseAccountId: "<id>",
    incomeAccountId: "<id>",
    inventoryStartDate: "<value>",
    itemNumber: "<value>",
    name: "<value>",
    priceIncludesTax: true,
    stockCount: 5489.99,
    taxCode: "<value>",
    taxRatePercentage: 4503.78,
    type: "SERVICE",
    unitName: "KILOGRAM",
    unitPurchasePrice: 7678.2,
    unitSalesPrice: 9663.3,
  },
};
```

## Fields

| Field                                                                  | Type                                                                   | Required                                                               | Description                                                            |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| `environmentName`                                                      | *string*                                                               | :heavy_minus_sign:                                                     | N/A                                                                    |
| `companyId`                                                            | *string*                                                               | :heavy_minus_sign:                                                     | N/A                                                                    |
| `xApiKey`                                                              | *string*                                                               | :heavy_minus_sign:                                                     | API key                                                                |
| `xAccountKey`                                                          | *string*                                                               | :heavy_minus_sign:                                                     | Account key                                                            |
| `body`                                                                 | [models.CreateItemRequestDto](../../models/create-item-request-dto.md) | :heavy_check_mark:                                                     | N/A                                                                    |