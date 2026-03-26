# PatchContactResponse

## Example Usage

```typescript
import { PatchContactResponse } from "@maesn/typescript-sdk/models/operations";

let value: PatchContactResponse = {
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

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `meta`                                                                              | [operations.PatchContactMeta](../../models/operations/patch-contact-meta.md)        | :heavy_minus_sign:                                                                  | N/A                                                                                 |
| `data`                                                                              | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)              | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `errors`                                                                            | [operations.PatchContactErrors](../../models/operations/patch-contact-errors.md)    | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `rawData`                                                                           | [operations.PatchContactRawData](../../models/operations/patch-contact-raw-data.md) | :heavy_check_mark:                                                                  | N/A                                                                                 |