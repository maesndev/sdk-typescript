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
  reference: "<value>",
  status: "VOIDED",
  taxText: "<value>",
  totalDiscountAmount: 2088.08,
  totalDiscountPercentage: 1042.39,
  totalGrossAmount: 2487.12,
  totalNetAmount: 6604.86,
  totalTaxAmount: null,
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
| `expirationDate`                                                               | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
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