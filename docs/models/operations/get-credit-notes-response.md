# GetCreditNotesResponse

## Example Usage

```typescript
import { GetCreditNotesResponse } from "maesn/models/operations";

let value: GetCreditNotesResponse = {
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
          addressLine1: "429 Walsh Tunnel",
          addressLine2: "-",
          city: "East Melyssa",
          countryCode: "AE",
          postalCode: "39193",
          type: "SELLING",
        },
      ],
      contactId: "<id>",
      createdDate: "<value>",
      creditNoteDate: "<value>",
      creditNoteLines: [],
      creditNoteNumber: "<value>",
      currency: "Peso Uruguayo",
      paymentStatus: "NO_OPEN_ITEM",
      paymentTermId: "<id>",
      reference: "<value>",
      status: "OVERDUE",
      totalDiscountAmount: 959.59,
      totalDiscountPercentage: 3781.27,
      totalGrossAmount: 624.21,
      totalNetAmount: 5542.24,
      totalTaxAmount: 9542.61,
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `meta`                                                                                   | [models.MetaResponse](../../models/meta-response.md)                                     | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `data`                                                                                   | [models.CreditNoteResponseDto](../../models/credit-note-response-dto.md)[]               | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `errors`                                                                                 | [operations.GetCreditNotesErrors](../../models/operations/get-credit-notes-errors.md)    | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `rawData`                                                                                | [operations.GetCreditNotesRawData](../../models/operations/get-credit-notes-raw-data.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |