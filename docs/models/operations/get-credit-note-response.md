# GetCreditNoteResponse

Credit note record matching the provided ID

## Example Usage

```typescript
import { GetCreditNoteResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetCreditNoteResponse = {
  data: {
    id: "<id>",
    addresses: [
      {},
    ],
    contactId: "<id>",
    createdDate: "<value>",
    creditNoteDate: "<value>",
    creditNoteLines: [
      {
        id: "<id>",
        createdDate: "<value>",
        description: "replacement swift mmm",
        itemId: "<id>",
        itemName: "<value>",
        quantity: 7964.31,
        taxCode: "<value>",
        taxRatePercentage: 2289.85,
        totalDiscountAmount: 2224.65,
        totalDiscountPercentage: 8636.87,
        totalGrossAmount: null,
        totalNetAmount: 8637.84,
        totalTaxAmount: 2022.47,
        type: "MATERIAL",
        unitAmount: 7633.55,
        unitDiscountAmount: null,
        unitDiscountPercentage: 5313.04,
        unitName: "<value>",
        updatedDate: null,
      },
    ],
    creditNoteNumber: "<value>",
    currency: "Burundi Franc",
    paymentStatus: "PENDING",
    paymentTermId: "<id>",
    reference: "<value>",
    status: "VOIDED",
    taxRatePercentage: 5039.64,
    taxRule: "INTRACOMMUNITY_GOODS",
    totalDiscountAmount: 732.08,
    totalDiscountPercentage: 8273.2,
    totalGrossAmount: 8820.33,
    totalNetAmount: 360.27,
    totalTaxAmount: 697.56,
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