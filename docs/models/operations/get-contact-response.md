# GetContactResponse

## Example Usage

```typescript
import { GetContactResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetContactResponse = {
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

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `meta`                                                                          | [operations.GetContactMeta](../../models/operations/get-contact-meta.md)        | :heavy_minus_sign:                                                              | N/A                                                                             |
| `data`                                                                          | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)          | :heavy_check_mark:                                                              | N/A                                                                             |
| `errors`                                                                        | [operations.GetContactErrors](../../models/operations/get-contact-errors.md)    | :heavy_check_mark:                                                              | N/A                                                                             |
| `rawData`                                                                       | [operations.GetContactRawData](../../models/operations/get-contact-raw-data.md) | :heavy_check_mark:                                                              | N/A                                                                             |