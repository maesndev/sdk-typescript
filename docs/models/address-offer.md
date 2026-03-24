# AddressOffer

## Example Usage

```typescript
import { AddressOffer } from "maesn/models";

let value: AddressOffer = {
  addressLine1: "1296 Isaias Wells",
  addressLine2: "-",
  city: "Port Maureen",
  countryCode: "GH",
  postalCode: "57261-0675",
  type: "DELIVERY",
};
```

## Fields

| Field                                                                     | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `addressLine1`                                                            | *string*                                                                  | :heavy_check_mark:                                                        | N/A                                                                       |
| `addressLine2`                                                            | *string*                                                                  | :heavy_check_mark:                                                        | N/A                                                                       |
| `city`                                                                    | *string*                                                                  | :heavy_check_mark:                                                        | N/A                                                                       |
| `countryCode`                                                             | [models.AddressOfferCountryCode](../models/address-offer-country-code.md) | :heavy_check_mark:                                                        | N/A                                                                       |
| `postalCode`                                                              | *string*                                                                  | :heavy_check_mark:                                                        | N/A                                                                       |
| `type`                                                                    | [models.AddressOfferType](../models/address-offer-type.md)                | :heavy_check_mark:                                                        | N/A                                                                       |