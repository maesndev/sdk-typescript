# GetCreditNotesResponse

List of credit notes for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetCreditNotesResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetCreditNotesResponse = {
  data: [
    {
      id: "<id>",
      addresses: [
        {},
      ],
      contactId: null,
      createdDate: "<value>",
      creditNoteDate: null,
      creditNoteLines: [],
      creditNoteNumber: "<value>",
      currency: "Taka",
      paymentStatus: "CREDIT_NOTE_CLEARED",
      paymentTermId: "<id>",
      reference: "<value>",
      status: "OPEN",
      taxRule: "EXPORT_GOODS",
      totalDiscountAmount: 6614.68,
      totalDiscountPercentage: 8754.9,
      totalGrossAmount: 8287.55,
      totalNetAmount: 5564.06,
      totalTaxAmount: 9288.7,
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
| `meta`                                                                                   | [operations.GetCreditNotesMeta](../../models/operations/get-credit-notes-meta.md)        | :heavy_minus_sign:                                                                       | N/A                                                                                      |
| `data`                                                                                   | [models.CreditNoteResponseDto](../../models/credit-note-response-dto.md)[]               | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `errors`                                                                                 | [operations.GetCreditNotesErrors](../../models/operations/get-credit-notes-errors.md)    | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `rawData`                                                                                | [operations.GetCreditNotesRawData](../../models/operations/get-credit-notes-raw-data.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |