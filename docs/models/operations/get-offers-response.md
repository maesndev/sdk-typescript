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
      contactId: "<id>",
      createdDate: "<value>",
      currency: "Pound Sterling",
      lineItems: [
        {
          id: "<id>",
          accountCode: "<value>",
          accountId: "<id>",
          createdDate: null,
          description:
            "hoot digitize peter emerge illiterate pecan internalise furthermore incidentally whup",
          itemId: "<id>",
          name: "<value>",
          quantity: 8994.86,
          taxCode: "<value>",
          taxRatePercentage: null,
          taxType: "<value>",
          type: "ACCOUNT",
          totalDiscountAmount: 3787.25,
          totalDiscountPercentage: 941.61,
          totalGrossAmount: 8928.34,
          totalNetAmount: 3345.46,
          totalTaxAmount: 1923.84,
          unitAmount: 4943.19,
          unitDiscountAmount: 2989.25,
          unitDiscountPercentage: 9129.2,
          unitName: "<value>",
          updatedDate: "<value>",
        },
      ],
      name: "<value>",
      offerDate: "<value>",
      offerNumber: "<value>",
      oneLineAddress: null,
      reference: null,
      status: "EXPIRED",
      taxText: "<value>",
      totalDiscountAmount: 7245.14,
      totalDiscountPercentage: 9885.34,
      totalGrossAmount: 9207.26,
      totalNetAmount: 2810.87,
      totalTaxAmount: 2523.35,
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