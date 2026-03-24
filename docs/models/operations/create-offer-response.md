# CreateOfferResponse

## Example Usage

```typescript
import { CreateOfferResponse } from "maesn/models/operations";

let value: CreateOfferResponse = {
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
  data: {
    id: "<id>",
    addresses: [
      {
        addressLine1: "64389 W 3rd Street",
        addressLine2: "-",
        city: "Pflugerville",
        countryCode: "FO",
        postalCode: "33874",
        type: "DELIVERY",
      },
    ],
    contactId: "<id>",
    createdDate: "<value>",
    currency: "Cordoba Oro",
    lineItems: [],
    name: "<value>",
    offerDate: "<value>",
    offerNumber: "<value>",
    oneLineAddress: "<value>",
    reference: "<value>",
    status: "DRAFT",
    taxText: "<value>",
    totalDiscountAmount: 5115.24,
    totalDiscountPercentage: 5411.49,
    totalGrossAmount: 1091.52,
    totalNetAmount: 5580.03,
    totalTaxAmount: 9709.05,
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `meta`                                                                            | [models.MetaResponse](../../models/meta-response.md)                              | :heavy_check_mark:                                                                | N/A                                                                               |
| `data`                                                                            | [models.OfferResponseDto](../../models/offer-response-dto.md)                     | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.CreateOfferErrors](../../models/operations/create-offer-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.CreateOfferRawData](../../models/operations/create-offer-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |