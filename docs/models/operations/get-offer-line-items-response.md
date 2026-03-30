# GetOfferLineItemsResponse

List of line items for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetOfferLineItemsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetOfferLineItemsResponse = {
  data: [
    {
      id: "<id>",
      accountCode: "<value>",
      accountId: "<id>",
      createdDate: "<value>",
      description:
        "aw delirious punctuation calmly monthly usually likewise uh-huh",
      itemId: "<id>",
      name: "<value>",
      quantity: 2487.13,
      taxCode: "<value>",
      taxRatePercentage: 8606.06,
      taxType: "<value>",
      type: "ITEM",
      totalDiscountAmount: 5233.91,
      totalDiscountPercentage: 1324.14,
      totalGrossAmount: 3681.02,
      totalNetAmount: 6925.94,
      totalTaxAmount: 9373.18,
      unitAmount: 7809.1,
      unitDiscountAmount: 1640.74,
      unitDiscountPercentage: 757.95,
      unitName: "<value>",
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `meta`                                                                                          | [operations.GetOfferLineItemsMeta](../../models/operations/get-offer-line-items-meta.md)        | :heavy_minus_sign:                                                                              | N/A                                                                                             |
| `data`                                                                                          | [models.OfferLineItemResponseDto](../../models/offer-line-item-response-dto.md)[]               | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `errors`                                                                                        | [operations.GetOfferLineItemsErrors](../../models/operations/get-offer-line-items-errors.md)    | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `rawData`                                                                                       | [operations.GetOfferLineItemsRawData](../../models/operations/get-offer-line-items-raw-data.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |