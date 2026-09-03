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
      offerNumber: "<value>",
      oneLineAddress: "<value>",
      reference: null,
      status: "DECLINED",
      taxText: "<value>",
      totalDiscountAmount: 4440.25,
      totalDiscountPercentage: 3812.24,
      totalGrossAmount: 7499.54,
      totalNetAmount: 2569.34,
      totalTaxAmount: 4680.06,
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