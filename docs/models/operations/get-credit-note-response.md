# GetCreditNoteResponse

Credit note record matching the provided ID

## Example Usage

```typescript
import { GetCreditNoteResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetCreditNoteResponse = {
  data: {
    id: "<id>",
    addresses: [],
    contactId: "<id>",
    createdDate: "<value>",
    creditNoteDate: "<value>",
    creditNoteLines: [],
    creditNoteNumber: "<value>",
    currency: "Czech Koruna",
    paymentStatus: "PARTLY_PAID",
    paymentTermId: null,
    reference: "<value>",
    status: "VOIDED",
    totalDiscountAmount: 3823.14,
    totalDiscountPercentage: null,
    totalGrossAmount: 5562.23,
    totalNetAmount: 3836.41,
    totalTaxAmount: null,
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `meta`                                                                                 | [operations.GetCreditNoteMeta](../../models/operations/get-credit-note-meta.md)        | :heavy_minus_sign:                                                                     | N/A                                                                                    |
| `data`                                                                                 | [models.CreditNoteResponseDto](../../models/credit-note-response-dto.md)               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `errors`                                                                               | [operations.GetCreditNoteErrors](../../models/operations/get-credit-note-errors.md)    | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `rawData`                                                                              | [operations.GetCreditNoteRawData](../../models/operations/get-credit-note-raw-data.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |