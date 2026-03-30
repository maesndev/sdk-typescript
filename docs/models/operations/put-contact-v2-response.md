# PutContactV2Response

Contact updated successfully

## Example Usage

```typescript
import { PutContactV2Response } from "@maesn/typescript-sdk/models/operations";

let value: PutContactV2Response = {
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
| `meta`                                                                               | [operations.PutContactV2Meta](../../models/operations/put-contact-v2-meta.md)        | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `data`                                                                               | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)               | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `errors`                                                                             | [operations.PutContactV2Errors](../../models/operations/put-contact-v2-errors.md)    | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `rawData`                                                                            | [operations.PutContactV2RawData](../../models/operations/put-contact-v2-raw-data.md) | :heavy_check_mark:                                                                   | N/A                                                                                  |