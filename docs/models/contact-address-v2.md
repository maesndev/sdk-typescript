# ContactAddressV2

## Example Usage

```typescript
import { ContactAddressV2 } from "@maesn/typescript-sdk/models";

let value: ContactAddressV2 = {
  addressLine1: "47526 Destiny Causeway",
  addressLine2: "-",
  city: "Carrollport",
  countryCode: "SO",
  postalCode: "93033-5782",
  type: "BILLING",
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `addressLine1`                                                                     | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `addressLine2`                                                                     | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `city`                                                                             | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `countryCode`                                                                      | [models.ContactAddressV2CountryCode](../models/contact-address-v2-country-code.md) | :heavy_check_mark:                                                                 | N/A                                                                                |
| `postalCode`                                                                       | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `type`                                                                             | [models.ContactAddressV2Type](../models/contact-address-v2-type.md)                | :heavy_check_mark:                                                                 | N/A                                                                                |