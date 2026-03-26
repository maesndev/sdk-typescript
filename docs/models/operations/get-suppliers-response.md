# GetSuppliersResponse

## Example Usage

```typescript
import { GetSuppliersResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetSuppliersResponse = {
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
| `meta`                                                                              | [operations.GetSuppliersMeta](../../models/operations/get-suppliers-meta.md)        | :heavy_minus_sign:                                                                  | N/A                                                                                 |
| `data`                                                                              | [models.ContactResponseDto](../../models/contact-response-dto.md)[]                 | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `errors`                                                                            | [operations.GetSuppliersErrors](../../models/operations/get-suppliers-errors.md)    | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `rawData`                                                                           | [operations.GetSuppliersRawData](../../models/operations/get-suppliers-raw-data.md) | :heavy_check_mark:                                                                  | N/A                                                                                 |