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
    contactId: "<id>",
    createdDate: "<value>",
    currency: "Dong",
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
    reference: "<value>",
    status: "DECLINED",
    taxText: "<value>",
    totalDiscountAmount: 3837.35,
    totalDiscountPercentage: 927.85,
    totalGrossAmount: null,
    totalNetAmount: 5411.49,
    totalTaxAmount: 5580.03,
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