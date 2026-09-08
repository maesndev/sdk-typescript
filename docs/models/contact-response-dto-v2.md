# ContactResponseDtoV2

## Example Usage

```typescript
import { ContactResponseDtoV2 } from "@maesn/typescript-sdk/models";

let value: ContactResponseDtoV2 = {
  id: "<id>",
  addresses: [],
  bankAccounts: [
    {
      id: "<id>",
      bankName: "<value>",
      bic: "<value>",
      code: "<value>",
      iban: "GR79009281188D13Z8985830473",
      number: 6633.57,
    },
  ],
  businessRegistrationNumber: "<value>",
  companyName: "White - Gusikowski",
  contactPersons: [],
  contactType: "COMPANY",
  createdDate: "<value>",
  emailAddresses: [],
  isCustomer: true,
  isSupplier: null,
  number: "<value>",
  parentId: "<id>",
  phoneNumbers: [],
  projectId: "<id>",
  updatedDate: "<value>",
  vatId: "<id>",
  website: "<value>",
};
```

## Fields

| Field                                                                                       | Type                                                                                        | Required                                                                                    | Description                                                                                 |
| ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| `id`                                                                                        | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `addresses`                                                                                 | [models.ContactAddressV2](../models/contact-address-v2.md)[]                                | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `bankAccounts`                                                                              | [models.BankAccountResponseCommonDtoV2](../models/bank-account-response-common-dto-v2.md)[] | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `businessRegistrationNumber`                                                                | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `companyName`                                                                               | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `contactPersons`                                                                            | [models.ContactPersonDtoV2](../models/contact-person-dto-v2.md)[]                           | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `contactType`                                                                               | [models.ContactResponseDtoV2ContactType](../models/contact-response-dto-v2-contact-type.md) | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `createdDate`                                                                               | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `emailAddresses`                                                                            | [models.EmailAddressV2](../models/email-address-v2.md)[]                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `isCustomer`                                                                                | *boolean*                                                                                   | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `isSupplier`                                                                                | *boolean*                                                                                   | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `number`                                                                                    | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `parentId`                                                                                  | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `phoneNumbers`                                                                              | [models.PhoneNumberV2](../models/phone-number-v2.md)[]                                      | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `projectId`                                                                                 | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `updatedDate`                                                                               | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `vatId`                                                                                     | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |
| `website`                                                                                   | *string*                                                                                    | :heavy_check_mark:                                                                          | N/A                                                                                         |