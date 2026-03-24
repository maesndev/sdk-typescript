# PatchContactRequest

## Example Usage

```typescript
import { PatchContactRequest } from "maesn/models/operations";

let value: PatchContactRequest = {
  contactId: "<id>",
  body: {
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
    companyName: "Watsica LLC",
    contactPersons: [],
    contactType: "COMPANY",
    emailAddresses: [],
    isCustomer: true,
    isSupplier: true,
    number: "<value>",
    phoneNumbers: [
      {
        number: "<value>",
        type: "LANDLINE",
      },
    ],
    projectId: "<id>",
    website: "<value>",
  },
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `contactId`                                                                       | *string*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `environmentName`                                                                 | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `companyId`                                                                       | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `xApiKey`                                                                         | *string*                                                                          | :heavy_minus_sign:                                                                | API key                                                                           |
| `xAccountKey`                                                                     | *string*                                                                          | :heavy_minus_sign:                                                                | Account key                                                                       |
| `body`                                                                            | [models.CreateContactRequestDtoV2](../../models/create-contact-request-dto-v2.md) | :heavy_check_mark:                                                                | N/A                                                                               |