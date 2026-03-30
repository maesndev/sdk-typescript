# CreateContactV2Response

Contact created successfully

## Example Usage

```typescript
import { CreateContactV2Response } from "@maesn/typescript-sdk/models/operations";

let value: CreateContactV2Response = {
  data: {
    id: "<id>",
    addresses: [],
    companyName: "Kuhn and Sons",
    contactPersons: [],
    contactType: "UNDEFINED",
    createdDate: "<value>",
    emailAddresses: [],
    isCustomer: false,
    isSupplier: false,
    number: "<value>",
    phoneNumbers: [
      {
        number: "<value>",
        type: "PRIVATE",
      },
    ],
    projectId: "<id>",
    updatedDate: "<value>",
    website: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `meta`                                                                                     | [operations.CreateContactV2Meta](../../models/operations/create-contact-v2-meta.md)        | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)                     | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.CreateContactV2Errors](../../models/operations/create-contact-v2-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.CreateContactV2RawData](../../models/operations/create-contact-v2-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |