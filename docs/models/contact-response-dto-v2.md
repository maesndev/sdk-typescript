# ContactResponseDtoV2

## Example Usage

```typescript
import { ContactResponseDtoV2 } from "maesn/models";

let value: ContactResponseDtoV2 = {
  id: "<id>",
  addresses: [
    {
      addressLine1: "8125 Jeffery Park",
      addressLine2: "-",
      city: "Ameliabury",
      countryCode: "CG",
      postalCode: "45430",
      type: "BILLING",
    },
  ],
  companyName: "Davis, Mayer and Morissette",
  contactPersons: [
    {
      id: "<id>",
      emailAddresses: [],
      firstName: "Marcella",
      lastName: "Langosh",
      phoneNumbers: [],
      salutation: "<value>",
    },
  ],
  contactType: "CONTACT_PERSON",
  createdDate: "<value>",
  emailAddresses: [],
  isCustomer: false,
  isSupplier: true,
  number: "<value>",
  phoneNumbers: [],
  projectId: "<id>",
  updatedDate: "<value>",
  website: "<value>",
};
```

## Fields

| Field                                                                                       | Type                                                                                        | Required                                                                                    | Description                                                                                 |
| ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| `id`                                                                                        | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `addresses`                                                                                 | [models.ContactAddress](../models/contact-address.md)[]                                     | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `companyName`                                                                               | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `contactPersons`                                                                            | [models.ContactPersonDtoV2](../models/contact-person-dto-v2.md)[]                           | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `contactType`                                                                               | [models.ContactResponseDtoV2ContactType](../models/contact-response-dto-v2-contact-type.md) | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `createdDate`                                                                               | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `emailAddresses`                                                                            | [models.EmailAddress](../models/email-address.md)[]                                         | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `isCustomer`                                                                                | *boolean*                                                                                   | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `isSupplier`                                                                                | *boolean*                                                                                   | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `number`                                                                                    | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `phoneNumbers`                                                                              | [models.PhoneNumber](../models/phone-number.md)[]                                           | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `projectId`                                                                                 | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `updatedDate`                                                                               | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `website`                                                                                   | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |