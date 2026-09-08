# ContactPersonDtoV2

## Example Usage

```typescript
import { ContactPersonDtoV2 } from "@maesn/typescript-sdk/models";

let value: ContactPersonDtoV2 = {
  id: "<id>",
  birthDate: "1979-08-17",
  emailAddresses: [],
  firstName: "Laron",
  jobTitle: "Regional Data Developer",
  lastName: "Stamm",
  phoneNumbers: [
    {
      number: "<value>",
      type: "OFFICE",
    },
  ],
  salutation: "<value>",
};
```

## Fields

| Field                                                    | Type                                                     | Required                                                 | Description                                              |
| -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- |
| `id`                                                     | *string*                                                 | :heavy_check_mark:                                       | N/A                                                      |
| `birthDate`                                              | *string*                                                 | :heavy_check_mark:                                       | N/A                                                      |
| `emailAddresses`                                         | [models.EmailAddressV2](../models/email-address-v2.md)[] | :heavy_check_mark:                                       | N/A                                                      |
| `firstName`                                              | *string*                                                 | :heavy_check_mark:                                       | N/A                                                      |
| `jobTitle`                                               | *string*                                                 | :heavy_check_mark:                                       | N/A                                                      |
| `lastName`                                               | *string*                                                 | :heavy_check_mark:                                       | N/A                                                      |
| `phoneNumbers`                                           | [models.PhoneNumberV2](../models/phone-number-v2.md)[]   | :heavy_check_mark:                                       | N/A                                                      |
| `salutation`                                             | *string*                                                 | :heavy_check_mark:                                       | N/A                                                      |