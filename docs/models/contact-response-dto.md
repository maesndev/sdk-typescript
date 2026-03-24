# ContactResponseDto

## Example Usage

```typescript
import { ContactResponseDto } from "maesn/models";

let value: ContactResponseDto = {
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
  accountNumber: 2628.54,
  bankAccounts: [],
  companyName: "Weimann - Stehr",
  contactPersons: [],
  contactType: "COMPANY",
  documentId: "<id>",
  emailAddresses: [
    {
      email: "Amira56@gmail.com",
      type: "PRIVATE",
    },
  ],
  number: "<value>",
  phoneNumbers: [],
  projectId: "<id>",
  role: "CUSTOMER",
  updatedDate: "<value>",
  vatId: "<id>",
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `id`                                                                                   | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `addresses`                                                                            | [models.ContactAddress](../models/contact-address.md)[]                                | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `accountNumber`                                                                        | *number*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `bankAccounts`                                                                         | [models.BankAccountResponse](../models/bank-account-response.md)[]                     | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `companyName`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `contactPersons`                                                                       | [models.ContactPerson](../models/contact-person.md)[]                                  | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `contactType`                                                                          | [models.ContactResponseDtoContactType](../models/contact-response-dto-contact-type.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `documentId`                                                                           | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `emailAddresses`                                                                       | [models.EmailAddress](../models/email-address.md)[]                                    | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `number`                                                                               | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `phoneNumbers`                                                                         | [models.PhoneNumber](../models/phone-number.md)[]                                      | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `projectId`                                                                            | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `role`                                                                                 | [models.ContactResponseDtoRole](../models/contact-response-dto-role.md)                | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `updatedDate`                                                                          | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `vatId`                                                                                | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |