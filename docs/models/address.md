# Address

## Example Usage

```typescript
import { Address } from "maesn/models";

let value: Address = {
  addressLine1: "58408 Destini Parkways",
  addressLine2: "-",
  city: "St. Louis Park",
  countryCode: "BF",
  postalCode: "23641-9567",
  type: "DELIVERY",
};
```

## Fields

| Field                                                          | Type                                                           | Required                                                       | Description                                                    |
| -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- |
| `addressLine1`                                                 | *string*                                                       | :heavy_check_mark:                                             | N/A                                                            |
| `addressLine2`                                                 | *string*                                                       | :heavy_check_mark:                                             | N/A                                                            |
| `city`                                                         | *string*                                                       | :heavy_check_mark:                                             | N/A                                                            |
| `countryCode`                                                  | [models.AddressCountryCode](../models/address-country-code.md) | :heavy_check_mark:                                             | N/A                                                            |
| `postalCode`                                                   | *string*                                                       | :heavy_check_mark:                                             | N/A                                                            |
| `type`                                                         | [models.AddressType](../models/address-type.md)                | :heavy_check_mark:                                             | N/A                                                            |