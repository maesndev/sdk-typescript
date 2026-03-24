# GetOfferLineItemResponse

## Example Usage

```typescript
import { GetOfferLineItemResponse } from "maesn/models/operations";

let value: GetOfferLineItemResponse = {
  meta: {
    warnings: [
      "<value 1>",
      "<value 2>",
    ],
    pagination: {
      total: 3438.77,
      perPage: 5109.63,
      currentPage: 2626.79,
      totalPages: 3561.84,
    },
  },
  data: [
    {
      id: "<id>",
      accountCode: "<value>",
      accountId: "<id>",
      createdDate: "<value>",
      description: "amongst round up communicate gah unless eek altruistic",
      itemId: "<id>",
      name: "<value>",
      quantity: 8850.6,
      taxCode: "<value>",
      taxRatePercentage: 6488.28,
      taxType: "<value>",
      type: "ITEM",
      totalDiscountAmount: 4527.48,
      totalDiscountPercentage: 8046.37,
      totalGrossAmount: 3685.62,
      totalNetAmount: 8710.16,
      totalTaxAmount: 7578.76,
      unitAmount: 2487.13,
      unitDiscountAmount: 8336.02,
      unitDiscountPercentage: 5107.77,
      unitName: "<value>",
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `meta`                                                                                        | [models.MetaResponse](../../models/meta-response.md)                                          | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `data`                                                                                        | [models.OfferLineItemResponseDto](../../models/offer-line-item-response-dto.md)[]             | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `errors`                                                                                      | [operations.GetOfferLineItemErrors](../../models/operations/get-offer-line-item-errors.md)    | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `rawData`                                                                                     | [operations.GetOfferLineItemRawData](../../models/operations/get-offer-line-item-raw-data.md) | :heavy_check_mark:                                                                            | N/A                                                                                           |