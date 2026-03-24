# OfferResponseDto

## Example Usage

```typescript
import { OfferResponseDto } from "maesn/models";

let value: OfferResponseDto = {
  id: "<id>",
  addresses: [],
  contactId: "<id>",
  createdDate: "<value>",
  currency: "Rufiyaa",
  lineItems: [],
  name: "<value>",
  offerDate: "<value>",
  offerNumber: "<value>",
  oneLineAddress: "<value>",
  reference: "<value>",
  status: "DECLINED",
  taxText: "<value>",
  totalDiscountAmount: 1875.79,
  totalDiscountPercentage: 4006.14,
  totalGrossAmount: 5995.29,
  totalNetAmount: 9579.52,
  totalTaxAmount: 8240.6,
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