# PutContactV2ResponseBody2

Contact created successfully (upsert)

## Example Usage

```typescript
import { PutContactV2ResponseBody2 } from "@maesn/typescript-sdk/models/operations";

let value: PutContactV2ResponseBody2 = {
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

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `meta`                                                                                 | [operations.PutContactV2Meta2](../../models/operations/put-contact-v2-meta2.md)        | :heavy_minus_sign:                                                                     | N/A                                                                                    |
| `data`                                                                                 | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)                 | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `errors`                                                                               | [operations.PutContactV2Errors2](../../models/operations/put-contact-v2-errors2.md)    | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `rawData`                                                                              | [operations.PutContactV2RawData2](../../models/operations/put-contact-v2-raw-data2.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |