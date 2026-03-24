# CreateOfferRequestDto

## Example Usage

```typescript
import { CreateOfferRequestDto } from "maesn/models";

let value: CreateOfferRequestDto = {
  addresses: [],
  contactId: "<id>",
  currency: "Trinidad and Tobago Dollar",
  lineItems: [],
  name: "<value>",
  offerDate: "<value>",
  offerNumber: "<value>",
  oneLineAddress: "<value>",
  reference: "<value>",
  status: "DECLINED",
  taxText: "<value>",
  totalDiscountAmount: 7678.98,
  totalDiscountPercentage: 7385.08,
  totalGrossAmount: 6891.77,
  totalNetAmount: 2412.81,
  totalTaxAmount: 7275.17,
};
```

## Fields

| Field                                                                                     | Type                                                                                      | Required                                                                                  | Description                                                                               |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `addresses`                                                                               | [models.AddressOffer](../models/address-offer.md)[]                                       | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `contactId`                                                                               | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `currency`                                                                                | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `lineItems`                                                                               | [models.CreateOfferLineItemRequestDto](../models/create-offer-line-item-request-dto.md)[] | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `name`                                                                                    | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `offerDate`                                                                               | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `offerNumber`                                                                             | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `oneLineAddress`                                                                          | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `reference`                                                                               | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `status`                                                                                  | [models.CreateOfferRequestDtoStatus](../models/create-offer-request-dto-status.md)        | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `taxText`                                                                                 | *string*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `totalDiscountAmount`                                                                     | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `totalDiscountPercentage`                                                                 | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `totalGrossAmount`                                                                        | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `totalNetAmount`                                                                          | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |
| `totalTaxAmount`                                                                          | *number*                                                                                  | :heavy_check_mark:                                                                        | N/A                                                                                       |