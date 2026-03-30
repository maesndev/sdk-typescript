# GetOfferLineItemResponse

Offer line item record matching the provided ID

## Example Usage

```typescript
import { GetOfferLineItemResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetOfferLineItemResponse = {
  data: {
    id: "<id>",
    accountCode: "<value>",
    accountId: "<id>",
    createdDate: "<value>",
    description: "yet as wherever state but gadzooks taxicab",
    itemId: "<id>",
    name: "<value>",
    quantity: 9465.37,
    taxCode: "<value>",
    taxRatePercentage: 708.1,
    taxType: "<value>",
    type: "FIXED_ASSET",
    totalDiscountAmount: 1898.26,
    totalDiscountPercentage: 6192.29,
    totalGrossAmount: 9294.03,
    totalNetAmount: 8474.43,
    totalTaxAmount: 9701.08,
    unitAmount: 5201.82,
    unitDiscountAmount: 7559.38,
    unitDiscountPercentage: 7342.71,
    unitName: "<value>",
    updatedDate: "<value>",
  },
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                                         | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `meta`                                                                                        | [operations.GetOfferLineItemMeta](../../models/operations/get-offer-line-item-meta.md)        | :heavy_minus_sign:                                                                            | N/A                                                                                           |
| `data`                                                                                        | [models.OfferLineItemResponseDto](../../models/offer-line-item-response-dto.md)               | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `errors`                                                                                      | [operations.GetOfferLineItemErrors](../../models/operations/get-offer-line-item-errors.md)    | :heavy_check_mark:                                                                            | N/A                                                                                           |
| `rawData`                                                                                     | [operations.GetOfferLineItemRawData](../../models/operations/get-offer-line-item-raw-data.md) | :heavy_check_mark:                                                                            | N/A                                                                                           |