# OfferResponseDto

## Example Usage

```typescript
import { OfferResponseDto } from "@maesn/typescript-sdk/models";

let value: OfferResponseDto = {
  id: "<id>",
  addresses: [],
  contactId: "<id>",
  createdDate: "<value>",
  currency: "Malaysian Ringgit",
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
  oneLineAddress: "<value>",
  reference: "<value>",
  status: "ACCEPTED",
  taxText: "<value>",
  totalDiscountAmount: 4544.44,
  totalDiscountPercentage: 6392.07,
  totalGrossAmount: 5483.87,
  totalNetAmount: 4385.89,
  totalTaxAmount: 43.22,
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                          | Type                                                                           | Required                                                                       | Description                                                                    |
| ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| `id`                                                                           | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `addresses`                                                                    | [models.AddressOffer](../models/address-offer.md)[]                            | :heavy_check_mark:                                                             | N/A                                                                            |
| `contactId`                                                                    | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `createdDate`                                                                  | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `currency`                                                                     | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `lineItems`                                                                    | [models.OfferLineItemResponseDto](../models/offer-line-item-response-dto.md)[] | :heavy_check_mark:                                                             | N/A                                                                            |
| `name`                                                                         | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `offerDate`                                                                    | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `offerNumber`                                                                  | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `oneLineAddress`                                                               | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `reference`                                                                    | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `status`                                                                       | [models.OfferResponseDtoStatus](../models/offer-response-dto-status.md)        | :heavy_check_mark:                                                             | N/A                                                                            |
| `taxText`                                                                      | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `totalDiscountAmount`                                                          | *number*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `totalDiscountPercentage`                                                      | *number*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `totalGrossAmount`                                                             | *number*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `totalNetAmount`                                                               | *number*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `totalTaxAmount`                                                               | *number*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `updatedDate`                                                                  | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |