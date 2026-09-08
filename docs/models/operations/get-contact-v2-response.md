# GetContactV2Response

Contact record matching the provided ID

## Example Usage

```typescript
import { GetContactV2Response } from "@maesn/typescript-sdk/models/operations";

let value: GetContactV2Response = {
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

| Field                                                                                | Type                                                                                 | Required                                                                             | Description                                                                          |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| `meta`                                                                               | [operations.GetContactV2Meta](../../models/operations/get-contact-v2-meta.md)        | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `data`                                                                               | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)               | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `errors`                                                                             | [operations.GetContactV2Errors](../../models/operations/get-contact-v2-errors.md)    | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `rawData`                                                                            | [operations.GetContactV2RawData](../../models/operations/get-contact-v2-raw-data.md) | :heavy_check_mark:                                                                   | N/A                                                                                  |