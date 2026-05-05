# PutContactV2ResponseBody1

Contact updated successfully

## Example Usage

```typescript
import { PutContactV2ResponseBody1 } from "@maesn/typescript-sdk/models/operations";

let value: PutContactV2ResponseBody1 = {
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

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `meta`                                                                                 | [operations.PutContactV2Meta1](../../models/operations/put-contact-v2-meta1.md)        | :heavy_minus_sign:                                                                     | N/A                                                                                    |
| `data`                                                                                 | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)                 | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `errors`                                                                               | [operations.PutContactV2Errors1](../../models/operations/put-contact-v2-errors1.md)    | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `rawData`                                                                              | [operations.PutContactV2RawData1](../../models/operations/put-contact-v2-raw-data1.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |