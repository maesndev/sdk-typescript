# UpdateCustomerResponse

Customer updated successfully

## Example Usage

```typescript
import { UpdateCustomerResponse } from "@maesn/typescript-sdk/models/operations";

let value: UpdateCustomerResponse = {
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
          {},
        ],
        firstName: "Devan",
        lastName: "Stark",
        phoneNumbers: [],
        salutation: "<value>",
      },
    ],
    contactType: "COMPANY",
    documentId: "<id>",
    emailAddresses: [],
    number: "<value>",
    phoneNumbers: [
      {},
    ],
    projectId: "<id>",
    role: "CUSTOMER",
    updatedDate: "<value>",
    vatId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `meta`                                                                                  | [operations.UpdateCustomerMeta](../../models/operations/update-customer-meta.md)        | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `data`                                                                                  | [models.ContactResponseDto](../../models/contact-response-dto.md)                       | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `errors`                                                                                | [operations.UpdateCustomerErrors](../../models/operations/update-customer-errors.md)    | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `rawData`                                                                               | [operations.UpdateCustomerRawData](../../models/operations/update-customer-raw-data.md) | :heavy_check_mark:                                                                      | N/A                                                                                     |