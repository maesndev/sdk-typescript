# GetContactV2Response

## Example Usage

```typescript
import { GetContactV2Response } from "@maesn/typescript-sdk/models/operations";

let value: GetContactV2Response = {
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

| Field                                                                                | Type                                                                                 | Required                                                                             | Description                                                                          |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| `meta`                                                                               | [operations.GetContactV2Meta](../../models/operations/get-contact-v2-meta.md)        | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `data`                                                                               | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)               | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `errors`                                                                             | [operations.GetContactV2Errors](../../models/operations/get-contact-v2-errors.md)    | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `rawData`                                                                            | [operations.GetContactV2RawData](../../models/operations/get-contact-v2-raw-data.md) | :heavy_check_mark:                                                                   | N/A                                                                                  |