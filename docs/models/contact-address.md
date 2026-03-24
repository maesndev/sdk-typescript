# ContactAddress

## Example Usage

```typescript
import { ContactAddress } from "maesn/models";

let value: ContactAddress = {
  addressLine1: "513 Homenick Glen",
  addressLine2: "-",
  city: "North Blaise",
  countryCode: "PF",
  postalCode: "85036-0715",
  type: "DELIVERY",
};
```

## Fields

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `addressLine1`                                                                | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `addressLine2`                                                                | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `city`                                                                        | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `countryCode`                                                                 | [models.ContactAddressCountryCode](../models/contact-address-country-code.md) | :heavy_check_mark:                                                            | N/A                                                                           |
| `postalCode`                                                                  | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `type`                                                                        | [models.ContactAddressType](../models/contact-address-type.md)                | :heavy_check_mark:                                                            | N/A                                                                           |