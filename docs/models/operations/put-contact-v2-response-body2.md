# PutContactV2ResponseBody2

Contact created successfully (upsert)

## Example Usage

```typescript
import { PutContactV2ResponseBody2 } from "@maesn/typescript-sdk/models/operations";

let value: PutContactV2ResponseBody2 = {
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
| `meta`                                                                                 | [operations.PutContactV2Meta2](../../models/operations/put-contact-v2-meta2.md)        | :heavy_minus_sign:                                                                     | N/A                                                                                    |
| `data`                                                                                 | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)                 | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `errors`                                                                               | [operations.PutContactV2Errors2](../../models/operations/put-contact-v2-errors2.md)    | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `rawData`                                                                              | [operations.PutContactV2RawData2](../../models/operations/put-contact-v2-raw-data2.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |