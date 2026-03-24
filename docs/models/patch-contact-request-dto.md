# PatchContactRequestDto

## Example Usage

```typescript
import { PatchContactRequestDto } from "maesn/models";

let value: PatchContactRequestDto = {
  contactType: "COMPANY",
  companyName: "Leuschke - Will",
  contactPersons: [
    {
      emailAddresses: [],
      firstName: "Layla",
      lastName: "Marks",
      phoneNumbers: [
        "<value 1>",
        "<value 2>",
        "<value 3>",
      ],
      salutation: "<value>",
    },
  ],
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
  emailAddresses: [],
  phoneNumbers: [
    {
      number: "<value>",
      type: "LANDLINE",
    },
  ],
  bankAccount: {
    iban: "XK760015004653009306",
    bic: "<value>",
    holder: "<value>",
    sepa: true,
  },
  projectId: "<id>",
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `contactType`                                                                                   | [models.PatchContactRequestDtoContactType](../models/patch-contact-request-dto-contact-type.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `companyName`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `contactPersons`                                                                                | [models.ContactPerson](../models/contact-person.md)[]                                           | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `addresses`                                                                                     | [models.ContactAddress](../models/contact-address.md)[]                                         | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `emailAddresses`                                                                                | [models.EmailAddress](../models/email-address.md)[]                                             | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `phoneNumbers`                                                                                  | [models.PhoneNumber](../models/phone-number.md)[]                                               | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `bankAccount`                                                                                   | [models.BankAccount](../models/bank-account.md)                                                 | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `projectId`                                                                                     | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |