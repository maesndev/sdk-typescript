# PatchSupplierRequest

## Example Usage

```typescript
import { PatchSupplierRequest } from "maesn/models/operations";

let value: PatchSupplierRequest = {
  contactId: "<id>",
  body: {
    contactType: "COMPANY",
    companyName: "Gerhold - Klocko",
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
  },
};
```

## Fields

| Field                                                                      | Type                                                                       | Required                                                                   | Description                                                                |
| -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| `contactId`                                                                | *string*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `environmentName`                                                          | *string*                                                                   | :heavy_minus_sign:                                                         | N/A                                                                        |
| `companyId`                                                                | *string*                                                                   | :heavy_minus_sign:                                                         | N/A                                                                        |
| `xApiKey`                                                                  | *string*                                                                   | :heavy_minus_sign:                                                         | API key                                                                    |
| `xAccountKey`                                                              | *string*                                                                   | :heavy_minus_sign:                                                         | Account key                                                                |
| `body`                                                                     | [models.PatchContactRequestDto](../../models/patch-contact-request-dto.md) | :heavy_check_mark:                                                         | N/A                                                                        |