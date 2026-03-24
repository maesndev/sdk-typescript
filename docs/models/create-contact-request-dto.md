# CreateContactRequestDto

## Example Usage

```typescript
import { CreateContactRequestDto } from "maesn/models";

let value: CreateContactRequestDto = {
  addresses: [],
  bankAccount: {
    bic: "<value>",
    holder: "<value>",
    isMainAccount: false,
    iban: "RO93SRKZ02P14477RS0T6A94",
    name: "<value>",
    sepa: true,
  },
  companyName: "Kovacek - Little",
  contactPersons: [],
  contactType: "CONTACT_PERSON",
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
  role: "SUPPLIER",
  vatId: "<id>",
};
```

## Fields

| Field                                                                                             | Type                                                                                              | Required                                                                                          | Description                                                                                       |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `addresses`                                                                                       | [models.CreateContactAddress](../models/create-contact-address.md)[]                              | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `bankAccount`                                                                                     | [models.CreateBankAccount](../models/create-bank-account.md)                                      | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `companyName`                                                                                     | *string*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `contactPersons`                                                                                  | [models.ContactPerson](../models/contact-person.md)[]                                             | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `contactType`                                                                                     | [models.CreateContactRequestDtoContactType](../models/create-contact-request-dto-contact-type.md) | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `documentId`                                                                                      | *string*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `emailAddresses`                                                                                  | [models.EmailAddress](../models/email-address.md)[]                                               | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `number`                                                                                          | *string*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `phoneNumbers`                                                                                    | [models.PhoneNumber](../models/phone-number.md)[]                                                 | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `projectId`                                                                                       | *string*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `role`                                                                                            | [models.CreateContactRequestDtoRole](../models/create-contact-request-dto-role.md)                | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `vatId`                                                                                           | *string*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |