# GetCustomersResponse

List of customers for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetCustomersResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetCustomersResponse = {
  data: [
    {
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
      companyName: "Prosacco and Sons",
      contactPersons: null,
      contactType: "CONTACT_PERSON",
      documentId: "<id>",
      emailAddresses: [],
      number: "<value>",
      phoneNumbers: [
        {
          number: "<value>",
          type: "OTHER",
        },
      ],
      projectId: "<id>",
      role: "CUSTOMER",
      updatedDate: null,
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `meta`                                                                              | [operations.GetCustomersMeta](../../models/operations/get-customers-meta.md)        | :heavy_minus_sign:                                                                  | N/A                                                                                 |
| `data`                                                                              | [models.ContactResponseDto](../../models/contact-response-dto.md)[]                 | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `errors`                                                                            | [operations.GetCustomersErrors](../../models/operations/get-customers-errors.md)    | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `rawData`                                                                           | [operations.GetCustomersRawData](../../models/operations/get-customers-raw-data.md) | :heavy_check_mark:                                                                  | N/A                                                                                 |