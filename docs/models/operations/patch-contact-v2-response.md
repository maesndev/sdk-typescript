# PatchContactV2Response

## Example Usage

```typescript
import { PatchContactV2Response } from "@maesn/typescript-sdk/models/operations";

let value: PatchContactV2Response = {
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
  rawData: null,
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `meta`                                                                                   | [operations.PatchContactV2Meta](../../models/operations/patch-contact-v2-meta.md)        | :heavy_minus_sign:                                                                       | N/A                                                                                      |
| `data`                                                                                   | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)                   | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `errors`                                                                                 | [operations.PatchContactV2Errors](../../models/operations/patch-contact-v2-errors.md)    | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `rawData`                                                                                | [operations.PatchContactV2RawData](../../models/operations/patch-contact-v2-raw-data.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |