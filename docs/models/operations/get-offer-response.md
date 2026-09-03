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
    expirationDate: "<value>",
    lineItems: [
      {
        id: "<id>",
        accountCode: "<value>",
        accountId: null,
        createdDate: "<value>",
        description:
          "gracefully sarong obsess jaggedly disadvantage guacamole well",
        itemId: "<id>",
        name: "<value>",
        quantity: 730.11,
        taxCode: "<value>",
        taxRatePercentage: 5122.1,
        taxType: "<value>",
        type: "SERVICE",
        totalDiscountAmount: 983.67,
        totalDiscountPercentage: 6658.39,
        totalGrossAmount: 2655.77,
        totalNetAmount: 8750.91,
        totalTaxAmount: 9870.2,
        unitAmount: 6984.27,
        unitDiscountAmount: 8994.86,
        unitDiscountPercentage: 705.72,
        unitName: "<value>",
        updatedDate: "<value>",
      },
    ],
    name: "<value>",
    offerDate: "<value>",
    offerNumber: null,
    oneLineAddress: "<value>",
    reference: "<value>",
    status: "VOIDED",
    taxText: "<value>",
    totalDiscountAmount: 6225.51,
    totalDiscountPercentage: null,
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