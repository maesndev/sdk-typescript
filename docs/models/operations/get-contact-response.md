# GetContactResponse

Contact record matching the provided ID

## Example Usage

```typescript
import { GetContactResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetContactResponse = {
  data: {
    id: "<id>",
    addresses: [],
    bankAccounts: [],
    businessRegistrationNumber: "<value>",
    companyName: "Bradtke, Klocko and Volkman",
    contactPersons: [
      {
        id: "<id>",
        birthDate: "1994-04-10",
        emailAddresses: [
          {
            email: "Theodora_Herman91@hotmail.com",
            type: "OTHER",
          },
        ],
        firstName: "Albert",
        jobTitle: "Dynamic Accountability Manager",
        lastName: "Christiansen",
        phoneNumbers: [
          {
            number: "<value>",
            type: "OFFICE",
          },
        ],
        salutation: "<value>",
      },
    ],
    contactType: "CONTACT_PERSON",
    createdDate: "<value>",
    emailAddresses: [
      {
        email: "Theodora_Herman91@hotmail.com",
        type: "OTHER",
      },
    ],
    isCustomer: false,
    isSupplier: true,
    number: "<value>",
    parentId: "<id>",
    phoneNumbers: [
      {
        number: "<value>",
        type: "OFFICE",
      },
    ],
    projectId: "<id>",
    updatedDate: "<value>",
    vatId: null,
    website: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `meta`                                                                          | [operations.GetContactMeta](../../models/operations/get-contact-meta.md)        | :heavy_minus_sign:                                                              | N/A                                                                             |
| `data`                                                                          | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)          | :heavy_check_mark:                                                              | N/A                                                                             |
| `errors`                                                                        | [operations.GetContactErrors](../../models/operations/get-contact-errors.md)    | :heavy_check_mark:                                                              | N/A                                                                             |
| `rawData`                                                                       | [operations.GetContactRawData](../../models/operations/get-contact-raw-data.md) | :heavy_check_mark:                                                              | N/A                                                                             |