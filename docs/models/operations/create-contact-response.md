# CreateContactResponse

Contact created successfully. Returns 202 with taskId if processed asynchronously.

## Example Usage

```typescript
import { CreateContactResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateContactResponse = {
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

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [operations.CreateContactMeta](../../models/operations/create-contact-meta.md)        | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `data`                                                                                | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)                | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.CreateContactErrors](../../models/operations/create-contact-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.CreateContactRawData](../../models/operations/create-contact-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |