# GetOfferResponse

Offer record matching the provided ID

## Example Usage

```typescript
import { GetOfferResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetOfferResponse = {
  data: {
    id: "<id>",
    addresses: [
      {},
    ],
    createdDate: "<value>",
    currency: "Trinidad and Tobago Dollar",
    lineItems: [
      {
        id: "<id>",
        accountCode: "<value>",
        accountId: "<id>",
        createdDate: "<value>",
        description: null,
        itemId: "<id>",
        name: "<value>",
        quantity: 4394.36,
        taxCode: "<value>",
        taxRatePercentage: 6281.26,
        taxType: "<value>",
        type: "ITEM",
        totalDiscountAmount: 2936.92,
        totalDiscountPercentage: 2768.35,
        totalGrossAmount: 2419.83,
        totalNetAmount: 7148.04,
        totalTaxAmount: null,
        unitAmount: 9628.05,
        unitDiscountAmount: 6093.33,
        unitDiscountPercentage: 6742.69,
        unitName: "<value>",
        updatedDate: "<value>",
      },
    ],
    name: "<value>",
    offerDate: "<value>",
    offerNumber: "<value>",
    oneLineAddress: "<value>",
    reference: null,
    status: "ACCEPTED",
    taxText: "<value>",
    totalDiscountAmount: 4666.69,
    totalDiscountPercentage: 6225.51,
    totalGrossAmount: null,
    totalNetAmount: null,
    totalTaxAmount: 5411.49,
    updatedDate: "<value>",
  },
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `meta`                                                                      | [operations.GetOfferMeta](../../models/operations/get-offer-meta.md)        | :heavy_minus_sign:                                                          | N/A                                                                         |
| `data`                                                                      | [models.OfferResponseDto](../../models/offer-response-dto.md)               | :heavy_check_mark:                                                          | N/A                                                                         |
| `errors`                                                                    | [operations.GetOfferErrors](../../models/operations/get-offer-errors.md)    | :heavy_check_mark:                                                          | N/A                                                                         |
| `rawData`                                                                   | [operations.GetOfferRawData](../../models/operations/get-offer-raw-data.md) | :heavy_check_mark:                                                          | N/A                                                                         |