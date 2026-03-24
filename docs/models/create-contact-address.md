# CreateContactAddress

## Example Usage

```typescript
import { CreateContactAddress } from "maesn/models";

let value: CreateContactAddress = {
  addressLine1: "846 Jerde Union",
  addressLine2: "-",
  city: "Ullrichstead",
  countryCode: "ZW",
  postalCode: "56006-1064",
  type: "PRIVATE",
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `addressLine1`                                                                             | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `addressLine2`                                                                             | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `city`                                                                                     | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `countryCode`                                                                              | [models.CreateContactAddressCountryCode](../models/create-contact-address-country-code.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `postalCode`                                                                               | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `type`                                                                                     | [models.CreateContactAddressType](../models/create-contact-address-type.md)                | :heavy_check_mark:                                                                         | N/A                                                                                        |