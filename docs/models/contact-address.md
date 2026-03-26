# ContactAddress

## Example Usage

```typescript
import { ContactAddress } from "@maesn/typescript-sdk/models";

let value: ContactAddress = {
  addressLine1: "2343 Donnie Circles",
  addressLine2: "-",
  city: "Sengerstead",
  countryCode: null,
  postalCode: "07152-6141",
  type: "BILLING",
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