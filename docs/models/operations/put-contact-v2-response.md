# PutContactV2Response

## Example Usage

```typescript
import { PutContactV2Response } from "maesn/models/operations";

let value: PutContactV2Response = {
  meta: {
    warnings: [
      "<value 1>",
      "<value 2>",
    ],
    pagination: {
      total: 3438.77,
      perPage: 5109.63,
      currentPage: 2626.79,
      totalPages: 3561.84,
    },
  },
  data: {
    id: "<id>",
    addresses: [],
    companyName: "Harber - Corkery",
    contactPersons: [],
    contactType: "COMPANY",
    createdDate: "<value>",
    emailAddresses: [
      {
        email: "Amira56@gmail.com",
        type: "PRIVATE",
      },
    ],
    isCustomer: false,
    isSupplier: true,
    number: "<value>",
    phoneNumbers: [],
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
| `meta`                                                                               | [models.MetaResponse](../../models/meta-response.md)                                 | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `data`                                                                               | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)               | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `errors`                                                                             | [operations.PutContactV2Errors](../../models/operations/put-contact-v2-errors.md)    | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `rawData`                                                                            | [operations.PutContactV2RawData](../../models/operations/put-contact-v2-raw-data.md) | :heavy_check_mark:                                                                   | N/A                                                                                  |