# GetSuppliersResponse

## Example Usage

```typescript
import { GetSuppliersResponse } from "maesn/models/operations";

let value: GetSuppliersResponse = {
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
  data: [
    {
      id: "<id>",
      addresses: [
        {
          addressLine1: "8125 Jeffery Park",
          addressLine2: "-",
          city: "Ameliabury",
          countryCode: "CG",
          postalCode: "45430",
          type: "BILLING",
        },
      ],
      accountNumber: 8475.89,
      bankAccounts: [
        {
          bic: "<value>",
          holder: "<value>",
          isMainAccount: false,
          iban: "MU89SZBR0318029709085684057MSV",
          name: "<value>",
          sepa: true,
        },
      ],
      companyName: "Abshire - Lebsack",
      contactPersons: [],
      contactType: "UNDEFINED",
      documentId: "<id>",
      emailAddresses: [
        {
          email: "Amira56@gmail.com",
          type: "PRIVATE",
        },
      ],
      number: "<value>",
      phoneNumbers: [],
      projectId: "<id>",
      role: "CONTACT",
      updatedDate: "<value>",
      vatId: "<id>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `meta`                                                                              | [models.MetaResponse](../../models/meta-response.md)                                | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `data`                                                                              | [models.ContactResponseDto](../../models/contact-response-dto.md)[]                 | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `errors`                                                                            | [operations.GetSuppliersErrors](../../models/operations/get-suppliers-errors.md)    | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `rawData`                                                                           | [operations.GetSuppliersRawData](../../models/operations/get-suppliers-raw-data.md) | :heavy_check_mark:                                                                  | N/A                                                                                 |