# CreateLineItemRequest

## Example Usage

```typescript
import { CreateLineItemRequest } from "maesn/models/operations";

let value: CreateLineItemRequest = {
  invoiceId: "<id>",
  body: {
    accountCode: "<value>",
    accountId: "<id>",
    description: "minor silky splendid gestate haze intermesh",
    dimensions: [
      {
        id: "<id>",
        categoryName: "<value>",
        name: "<value>",
      },
    ],
    discountItemPercentage: 3616.16,
    grossAmount: 3638.49,
    itemId: "<id>",
    name: "<value>",
    quantity: 8433.27,
    taxCode: "<value>",
    taxRatePercentage: 6265.76,
    taxType: "<value>",
    type: "<value>",
    unitAmount: 413.75,
    unitName: "<value>",
  },
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `invoiceId`                                                                     | *string*                                                                        | :heavy_check_mark:                                                              | N/A                                                                             |
| `environmentName`                                                               | *string*                                                                        | :heavy_minus_sign:                                                              | N/A                                                                             |
| `companyId`                                                                     | *string*                                                                        | :heavy_minus_sign:                                                              | N/A                                                                             |
| `xApiKey`                                                                       | *string*                                                                        | :heavy_minus_sign:                                                              | API key                                                                         |
| `xAccountKey`                                                                   | *string*                                                                        | :heavy_minus_sign:                                                              | Account key                                                                     |
| `body`                                                                          | [models.CreateLineItemRequestDto](../../models/create-line-item-request-dto.md) | :heavy_check_mark:                                                              | N/A                                                                             |