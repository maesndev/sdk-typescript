# OfferResponseDto

## Example Usage

```typescript
import { OfferResponseDto } from "@maesn/typescript-sdk/models";

let value: OfferResponseDto = {
  id: "<id>",
  addresses: [],
  createdDate: "<value>",
  currency: "Iranian Rial",
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
  status: "DRAFT",
  taxText: "<value>",
  totalDiscountAmount: 2777.54,
  totalDiscountPercentage: 2088.08,
  totalGrossAmount: 1042.39,
  totalNetAmount: 2487.12,
  totalTaxAmount: 6604.86,
  updatedDate: null,
};
```

## Fields

| Field                                                                          | Type                                                                           | Required                                                                       | Description                                                                    |
| ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| `id`                                                                           | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `addresses`                                                                    | [models.AddressOffer](../models/address-offer.md)[]                            | :heavy_check_mark:                                                             | N/A                                                                            |
| `contactId`                                                                    | *string*                                                                       | :heavy_minus_sign:                                                             | N/A                                                                            |
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