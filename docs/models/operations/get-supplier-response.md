# GetSupplierResponse

## Example Usage

```typescript
import { GetSupplierResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetSupplierResponse = {
  data: {
    id: "<id>",
    addresses: [
      {
        addressLine1: "62455 Fay Crossroad",
        addressLine2: null,
        city: "Hirambury",
        countryCode: null,
        postalCode: null,
        type: "PRIVATE",
      },
    ],
    companyName: "Hauck - Nitzsche",
    contactPersons: [
      {
        emailAddresses: [
          {
            email: "Queen25@gmail.com",
            type: "INVOICE",
          },
        ],
        firstName: "Name",
        lastName: null,
        phoneNumbers: [
          {
            number: "<value>",
            type: "OTHER",
          },
        ],
        salutation: "<value>",
      },
    ],
    contactType: "CONTACT_PERSON",
    documentId: "<id>",
    emailAddresses: [
      {
        email: "Queen25@gmail.com",
        type: "INVOICE",
      },
    ],
    number: "<value>",
    phoneNumbers: [],
    projectId: "<id>",
    role: "CUSTOMER",
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `meta`                                                                            | [operations.GetSupplierMeta](../../models/operations/get-supplier-meta.md)        | :heavy_minus_sign:                                                                | N/A                                                                               |
| `data`                                                                            | [models.ContactResponseDto](../../models/contact-response-dto.md)                 | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetSupplierErrors](../../models/operations/get-supplier-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetSupplierRawData](../../models/operations/get-supplier-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |