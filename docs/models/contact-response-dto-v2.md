# ContactResponseDtoV2

## Example Usage

```typescript
import { ContactResponseDtoV2 } from "@maesn/typescript-sdk/models";

let value: ContactResponseDtoV2 = {
  id: "<id>",
  addresses: [],
  companyName: "Purdy Inc",
  contactPersons: [],
  contactType: "COMPANY",
  createdDate: "<value>",
  emailAddresses: [
    {
      email: "Van72@gmail.com",
      type: "OTHER",
    },
  ],
  isCustomer: true,
  isSupplier: true,
  number: "<value>",
  phoneNumbers: [
    {
      number: "<value>",
      type: "PRIVATE",
    },
  ],
  projectId: "<id>",
  updatedDate: "<value>",
  website: "<value>",
};
```

## Fields

| Field                                                                                       | Type                                                                                        | Required                                                                                    | Description                                                                                 |
| ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| `id`                                                                                        | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `addresses`                                                                                 | [models.ContactAddressV2](../models/contact-address-v2.md)[]                                | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `companyName`                                                                               | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `contactPersons`                                                                            | [models.ContactPersonDtoV2](../models/contact-person-dto-v2.md)[]                           | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `contactType`                                                                               | [models.ContactResponseDtoV2ContactType](../models/contact-response-dto-v2-contact-type.md) | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `createdDate`                                                                               | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `emailAddresses`                                                                            | [models.EmailAddressV2](../models/email-address-v2.md)[]                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `isCustomer`                                                                                | *boolean*                                                                                   | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `isSupplier`                                                                                | *boolean*                                                                                   | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `number`                                                                                    | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `phoneNumbers`                                                                              | [models.PhoneNumberV2](../models/phone-number-v2.md)[]                                      | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `projectId`                                                                                 | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `updatedDate`                                                                               | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `website`                                                                                   | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |