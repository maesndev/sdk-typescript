# GetOffersResponse

List of offers for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetOffersResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetOffersResponse = {
  data: [
    {
      id: "<id>",
      addresses: [],
      createdDate: "<value>",
      currency: "East Caribbean Dollar",
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
      reference: "<value>",
      status: "VOIDED",
      taxText: "<value>",
      totalDiscountAmount: 3893.29,
      totalDiscountPercentage: 4850.17,
      totalGrossAmount: 5793.19,
      totalNetAmount: null,
      totalTaxAmount: 6527.2,
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `meta`                                                                        | [operations.GetOffersMeta](../../models/operations/get-offers-meta.md)        | :heavy_minus_sign:                                                            | N/A                                                                           |
| `data`                                                                        | [models.OfferResponseDto](../../models/offer-response-dto.md)[]               | :heavy_check_mark:                                                            | N/A                                                                           |
| `errors`                                                                      | [operations.GetOffersErrors](../../models/operations/get-offers-errors.md)    | :heavy_check_mark:                                                            | N/A                                                                           |
| `rawData`                                                                     | [operations.GetOffersRawData](../../models/operations/get-offers-raw-data.md) | :heavy_check_mark:                                                            | N/A                                                                           |