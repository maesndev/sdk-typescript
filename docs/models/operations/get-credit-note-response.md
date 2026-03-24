# GetCreditNoteResponse

## Example Usage

```typescript
import { GetCreditNoteResponse } from "maesn/models/operations";

let value: GetCreditNoteResponse = {
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
    currency: "Chilean Peso",
    paymentStatus: "CREDIT_NOTE_CLEARED",
    paymentTermId: "<id>",
    reference: "<value>",
    status: "PARTIALLY_OVERDUE",
    totalDiscountAmount: 4791.6,
    totalDiscountPercentage: 9713.96,
    totalGrossAmount: 3338.5,
    totalNetAmount: 7472.42,
    totalTaxAmount: 5206.48,
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `meta`                                                                                 | [models.MetaResponse](../../models/meta-response.md)                                   | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `data`                                                                                 | [models.CreditNoteResponseDto](../../models/credit-note-response-dto.md)               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `errors`                                                                               | [operations.GetCreditNoteErrors](../../models/operations/get-credit-note-errors.md)    | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `rawData`                                                                              | [operations.GetCreditNoteRawData](../../models/operations/get-credit-note-raw-data.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |