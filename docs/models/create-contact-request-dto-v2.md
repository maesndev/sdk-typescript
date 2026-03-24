# CreateContactRequestDtoV2

## Example Usage

```typescript
import { CreateContactRequestDtoV2 } from "maesn/models";

let value: CreateContactRequestDtoV2 = {
  id: "<id>",
  addresses: [
    {
      addressLine1: "321 McLaughlin Village",
      addressLine2: "-",
      city: "Lake Celiafield",
      countryCode: "NA",
      postalCode: "56972-1641",
      type: "EMPTY",
    },
  ],
  companyName: "Wilderman - Kovacek",
  contactPersons: [],
  contactType: "UNDEFINED",
  emailAddresses: [],
  isCustomer: true,
  isSupplier: false,
  number: "<value>",
  phoneNumbers: [
    {
      number: "<value>",
      type: "LANDLINE",
    },
  ],
  projectId: "<id>",
  website: "<value>",
};
```

## Fields

| Field                                                                                                  | Type                                                                                                   | Required                                                                                               | Description                                                                                            |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ |
| `id`                                                                                                   | *string*                                                                                               | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `addresses`                                                                                            | [models.CreateContactAddress](../models/create-contact-address.md)[]                                   | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `companyName`                                                                                          | *string*                                                                                               | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `contactPersons`                                                                                       | [models.CreateContactPersonDtoV2](../models/create-contact-person-dto-v2.md)[]                         | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `contactType`                                                                                          | [models.CreateContactRequestDtoV2ContactType](../models/create-contact-request-dto-v2-contact-type.md) | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `emailAddresses`                                                                                       | [models.EmailAddress](../models/email-address.md)[]                                                    | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `isCustomer`                                                                                           | *boolean*                                                                                              | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `isSupplier`                                                                                           | *boolean*                                                                                              | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `number`                                                                                               | *string*                                                                                               | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `phoneNumbers`                                                                                         | [models.PhoneNumber](../models/phone-number.md)[]                                                      | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `projectId`                                                                                            | *string*                                                                                               | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `website`                                                                                              | *string*                                                                                               | :heavy_check_mark:                                                                                     | N/A                                                                                                    |