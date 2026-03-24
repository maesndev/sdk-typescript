# GetOffersResponse

## Example Usage

```typescript
import { GetOffersResponse } from "maesn/models/operations";

let value: GetOffersResponse = {
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
      addresses: [],
      contactId: "<id>",
      createdDate: "<value>",
      currency: "Denar",
      lineItems: [],
      name: "<value>",
      offerDate: "<value>",
      offerNumber: "<value>",
      oneLineAddress: "<value>",
      reference: "<value>",
      status: "DECLINED",
      taxText: "<value>",
      totalDiscountAmount: 8443.53,
      totalDiscountPercentage: 9423.08,
      totalGrossAmount: 2862.95,
      totalNetAmount: 5540.74,
      totalTaxAmount: 9618.53,
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
| `meta`                                                                        | [models.MetaResponse](../../models/meta-response.md)                          | :heavy_check_mark:                                                            | N/A                                                                           |
| `data`                                                                        | [models.OfferResponseDto](../../models/offer-response-dto.md)[]               | :heavy_check_mark:                                                            | N/A                                                                           |
| `errors`                                                                      | [operations.GetOffersErrors](../../models/operations/get-offers-errors.md)    | :heavy_check_mark:                                                            | N/A                                                                           |
| `rawData`                                                                     | [operations.GetOffersRawData](../../models/operations/get-offers-raw-data.md) | :heavy_check_mark:                                                            | N/A                                                                           |