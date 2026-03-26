# ContactResponseDto

## Example Usage

```typescript
import { ContactResponseDto } from "@maesn/typescript-sdk/models";

let value: ContactResponseDto = {
  id: "<id>",
  addresses: [],
  companyName: "Stehr, Hermann and Kautzer",
  contactPersons: [],
  contactType: "UNDEFINED",
  documentId: null,
  emailAddresses: [],
  number: "<value>",
  phoneNumbers: [],
  projectId: "<id>",
  role: "CONTACT",
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `id`                                                                                   | *string*                                                                               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `addresses`                                                                            | [models.ContactAddress](../models/contact-address.md)[]                                | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `accountNumber`                                                                        | *number*                                                                               | :heavy_minus_sign:                                                                     | N/A                                                                                    |
| `bankAccounts`                                                                         | [models.BankAccountResponse](../models/bank-account-response.md)[]                     | :heavy_minus_sign:                                                                     | N/A                                                                                    |
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
| `vatId`                                                                                | *string*                                                                               | :heavy_minus_sign:                                                                     | N/A                                                                                    |