# ContactPersonDtoV2

## Example Usage

```typescript
import { ContactPersonDtoV2 } from "@maesn/typescript-sdk/models";

let value: ContactPersonDtoV2 = {
  id: "<id>",
  emailAddresses: [
    {
      email: "Van72@gmail.com",
      type: "OTHER",
    },
  ],
  firstName: "Faustino",
  lastName: "Grant",
  phoneNumbers: [
    {
      number: "<value>",
      type: "PRIVATE",
    },
  ],
  salutation: "<value>",
};
```

## Fields

| Field                                                    | Type                                                     | Required                                                 | Description                                              |
| -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- |
| `id`                                                     | *string*                                                 | :heavy_check_mark:                                       | N/A                                                      |
| `emailAddresses`                                         | [models.EmailAddressV2](../models/email-address-v2.md)[] | :heavy_check_mark:                                       | N/A                                                      |
| `firstName`                                              | *string*                                                 | :heavy_check_mark:                                       | N/A                                                      |
| `lastName`                                               | *string*                                                 | :heavy_check_mark:                                       | N/A                                                      |
| `phoneNumbers`                                           | [models.PhoneNumberV2](../models/phone-number-v2.md)[]   | :heavy_check_mark:                                       | N/A                                                      |
| `salutation`                                             | *string*                                                 | :heavy_check_mark:                                       | N/A                                                      |