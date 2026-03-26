# CreateCustomerRequest

## Example Usage

```typescript
import { CreateCustomerRequest } from "maesn/models/operations";

let value: CreateCustomerRequest = {
  body: {
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
    bankAccount: {
      bic: "<value>",
      holder: "<value>",
      isMainAccount: false,
      iban: "RO93SRKZ02P14477RS0T6A94",
      name: "<value>",
      sepa: true,
    },
    companyName: "Dickinson, Bogan and Bailey",
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
    contactType: "CONTACT_PERSON",
    documentId: "<id>",
    emailAddresses: [],
    number: "<value>",
    phoneNumbers: [],
    projectId: "<id>",
    role: "SUPPLIER",
    vatId: "<id>",
  },
};
```

## Fields

| Field                                                                        | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `environmentName`                                                            | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `companyId`                                                                  | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `body`                                                                       | [models.CreateContactRequestDto](../../models/create-contact-request-dto.md) | :heavy_check_mark:                                                           | N/A                                                                          |