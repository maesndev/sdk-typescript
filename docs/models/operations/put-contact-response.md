# PutContactResponse

## Example Usage

```typescript
import { PutContactResponse } from "@maesn/typescript-sdk/models/operations";

let value: PutContactResponse = {
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
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `meta`                                                                          | [operations.PutContactMeta](../../models/operations/put-contact-meta.md)        | :heavy_minus_sign:                                                              | N/A                                                                             |
| `data`                                                                          | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)          | :heavy_check_mark:                                                              | N/A                                                                             |
| `errors`                                                                        | [operations.PutContactErrors](../../models/operations/put-contact-errors.md)    | :heavy_check_mark:                                                              | N/A                                                                             |
| `rawData`                                                                       | [operations.PutContactRawData](../../models/operations/put-contact-raw-data.md) | :heavy_check_mark:                                                              | N/A                                                                             |