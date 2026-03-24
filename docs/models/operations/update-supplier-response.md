# UpdateSupplierResponse

## Example Usage

```typescript
import { UpdateSupplierResponse } from "maesn/models/operations";

let value: UpdateSupplierResponse = {
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
    accountNumber: 5053.75,
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
    companyName: "Gorczany - Hauck",
    contactPersons: [
      {
        emailAddresses: [],
        firstName: "Layla",
        lastName: "Marks",
        phoneNumbers: [
          "<value 1>",
          "<value 2>",
          "<value 3>",
        ],
        salutation: "<value>",
      },
    ],
    contactType: "COMPANY",
    documentId: "<id>",
    emailAddresses: [
      {
        email: "Amira56@gmail.com",
        type: "PRIVATE",
      },
    ],
    number: "<value>",
    phoneNumbers: [
      {
        number: "<value>",
        type: "LANDLINE",
      },
    ],
    projectId: "<id>",
    role: "SUPPLIER",
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
| `meta`                                                                                  | [models.MetaResponse](../../models/meta-response.md)                                    | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `data`                                                                                  | [models.ContactResponseDto](../../models/contact-response-dto.md)                       | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `errors`                                                                                | [operations.UpdateSupplierErrors](../../models/operations/update-supplier-errors.md)    | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `rawData`                                                                               | [operations.UpdateSupplierRawData](../../models/operations/update-supplier-raw-data.md) | :heavy_check_mark:                                                                      | N/A                                                                                     |